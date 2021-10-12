## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0
class Estudiante {
	{static} -matricula
	-nombres
	-apellido
	-semestreActual
	-campus
}

class Coordinador {
	-nombres
	-apellido
	{static} -nomina
	-campus
}

class Adminstrador {
	-nombres
	-apellido
	-edad
	{static} -id
	-campus
}

@enduml
```