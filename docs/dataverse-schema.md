# Dataverse Schema

## IT-Tickets

Main table used for IT support requests.

| Column | Type | Purpose |
|---|---|---|
| Titel | Text | Ticket title |
| Problem | Text | Problem description |
| Priority | Choice | Ticket priority |
| Status | Choice | Ticket status |
| Mitarbeiter | Lookup | Employee who submitted the ticket |
| Assigned To | Lookup | IT employee responsible for the ticket |

## Mitarbeiters

Employee table used for employee validation and ticket relationships.

| Column | Type | Purpose |
|---|---|---|
| E-Mail | Text | Employee email address |
| Name | Text | Employee name |

## Relationships

`IT-Tickets.Mitarbeiter` references `Mitarbeiters`.

`IT-Tickets.Assigned To` references `Mitarbeiters`.
