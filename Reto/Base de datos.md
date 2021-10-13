## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0

class Campus <<(C,white)>> {
	{static} -Int id
	-String nombre
}
class Adminstrador <<(A,white)>> {
	{static} -Int id
	-String nombres
	-String apellido
}
class Coordinador <<(C,white)>> {
	{static} -String nomina
	-String nombres
	-String apellido
	{abstract} -Int campusId
}
class Estudiante <<(E,white)>> {
	{static} - String matricula
	-String nombres
	-String apellido
	-Int tetraActual
	{abstract} -Int campusId
	{abstract} -Class TalleresInscritos
}
class Taller <<(T,white)>> {
    {static} -Int id 
    - String nombre
	- String Descripcion
    - String status
    - String image
}
class TalleresDisponibles <<(T, white)>> {
	{static} -String id
	{abstract} -Int tallerId
	{abstract} -Int campusId
	-Timestamp tiempoInicio
	-Timestamp tiempoFin
}
class TalleresInscritos <<(T,white)>> {
	{static} -registroId 
	{abstract} -String tallerId
	-String status
}









TalleresInscritos "1" <-- "1" Estudiante::TalleresInscritos
TalleresInscritos::tallerId "*" --> "1" TalleresDisponibles::id
TalleresDisponibles::tallerId "*" --> "1" Taller::id
Campus::id "*" <-- "1" TalleresDisponibles::campusId
Estudiante::campusId "*" --> "1" Campus::id
Coordinador::campusId "*" --> "1" Campus::id 

@enduml
```