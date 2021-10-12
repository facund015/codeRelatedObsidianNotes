## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0
class Estudiante {
	{static} -matricula
	-nombres
	-apellido
	-edad
	-semestreActual
	-campus
}

class Coordinador {
	-nombres
	-apellido
	-edad
	{static} -nomina
	-campus
}

class Adminstrador {
	-nombres
	-apellido
	-edad
	{static} -nomina
	-campus
}

@enduml
```