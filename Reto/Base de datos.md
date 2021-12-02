## Diagrama de clases
```plantuml
@startuml
skinparam classAttributeIconSize 0

class Users <<(U,white)>> {
	-{static} String Id
	-String Name
	-String Last_name
	-String Email
	-String Role
	-String Current_period
	{abstract} -String Campus_id
}

class Campus <<(C,white)>> {
	{static} -Int id
	-String name
}

class Period <<(P,white)>> {
	{static} -Int Id
	-String Name
	-Bool Current_period
}

class Workshop <<(W,white)>> {
	{static} -String Id
	-String Name
	-String Description
	-String Image
	-String Requirement
}
class Available_workshop <<(T, white)>> {
	{static} -String Id
	{abstract} -String Campus_id
	{abstract} -String Workshop_id
	{abstract} -String Period
	-Timestamp Start_time
	-Timestamp End_time
}
class TalleresInscritos <<(T,white)>> {
	{static} -Int registroId 
	{abstract} -String studentId
	{abstract} -String tallerId
	-String status
	-Int Calificacion
}

Users::Id "1" <-- "*" TalleresInscritos::studentId
Users::Campus_id "*" --> "1" Campus::id
Available_workshop::Id "1" <-- "*" TalleresInscritos::tallerId
//Available_workshop::Campus_id "1" -->  "*" Campus::id
Available_workshop::Workshop_id "*" --> "1" Workshop::Id




@enduml
```