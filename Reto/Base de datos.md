## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0
class Estudiante {
	{} -matricula
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
	-nomina
	-campus
}

class Adminstrador {
	-nombres
	-apellido
	-edad
	-nomina
	-campus
}

@enduml
```