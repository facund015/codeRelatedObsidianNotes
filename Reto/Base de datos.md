## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0
class Estudiante {
	{static} - String matricula
	-String nombres
	-String apellido
	-Int tetraActual
	-Int campusId
	-Class TalleresInscritos
}

class TalleresInscritos {
	{static} -registroId 
	{abstract} -Int tallerId
	-String status
}

class Coordinador {
	{static} -String nomina
	-String nombres
	-String apellido
	-Int campusId
}

class Taller {
    {static} -Int id 
    - String nombre
    - String status
    - String image
}

class Campus {
	{static} -Int id
	-String nombre
}

class Adminstrador {
	{static} -Int id
	-String nombres
	-String apellido
}

Estudiante::TalleresInscritos --> TalleresInscritos
TalleresInscritos::tallerId --> Taller::id
Estudiante::campusId --> Campus::id
Coordinador::campusId --> Campus::id 


@enduml
```