# SAP RAP Urlaubsantragsverwaltung

**Entwickelt von: Revathi Krishnamoorthy**

Dieses Projekt demonstriert eine **RAP-basierte SAP Anwendung** zur Verwaltung von Urlaubsanträgen mit **ABAP Cloud und Fiori Elements**.

## Funktionen

- RAP Business Object mit Draft-Funktion
- Implementierung von Determinations und Validations
- Workflow-Aktionen: **Submit, Approve, Reject**
- Instance Feature Control für die Aktivierung von Aktionen
- Value Help (Dropdown) für Leave Types
- OData V4 Service Binding
- Fiori Elements Benutzeroberfläche

## Verwendete Technologien

- ABAP Cloud
- RAP (RESTful Application Programming Model)
- CDS Views
- OData V4
- Fiori Elements
- ABAP Objects

## Geschäftslogik

Statuswerte im Workflow:

- `N` = New
- `S` = Submitted
- `A` = Approved
- `R` = Rejected

## Screenshots

### 1. Listenansicht der Anwendung
![List Page](screenshots/01_list_page.png)

### 2. Erstellung eines neuen Urlaubsantrags
![Create Form](screenshots/02_create_form.png)

### 3. Value Help für Leave Type
![Value Help](screenshots/03_value_help.png)

### 4. Antrag nach dem Submit
![Submitted](screenshots/04_submitted_status.png)

### 5. Genehmigter Antrag
![Approved](screenshots/05_approved_status.png)

### 6. Feature Control (Aktivierte/Deaktivierte Aktionen)
![Feature Control](screenshots/06_feature_control.png)

### 7. Behavior Definition (RAP)
![Behavior Definition](screenshots/07_behavior_definition.png)

### 8. CDS Projection View
![CDS View](screenshots/08_cds_view.png)

### 9. Handler Klasse (Actions)
![Handler Actions](screenshots/09_handler_actions.png)
