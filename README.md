# SAP RAP Urlaubsantragsverwaltung

**Entwickelt von: Revathi Krishnamoorthy**
GitHub: https://github.com/revathikrishnamoorthy-sap/sap-rap-leave-request-management

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

## Projektstruktur

Der Quellcode der Anwendung ist in folgende Bereiche unterteilt:

- **tables/** – Datenbanktabellen für Leave Requests und Value Help
- **cds/** – CDS Views für Datenmodellierung und Projektion
- **behavior/** – Behavior Definition für RAP Business Object
- **handler/** – Implementierung der Business Logik (Actions, Validations, Determinations)
- **screenshots/** – Screenshots der Fiori Anwendung

  ## Architektur der Anwendung

Die Anwendung basiert auf dem **SAP RESTful Application Programming Model (RAP)** und folgt einer klaren Schichtenstruktur:

1. **Datenbanktabellen**
   - Persistente Tabellen für Urlaubsanträge und Value Help Daten

2. **CDS Views**
   - Interface View zur Datenmodellierung
   - Projection View für die Bereitstellung an die UI
   - Value Help CDS für die Leave-Type-Auswahl

3. **Behavior Definition**
   - Definition des RAP Business Objects
   - Festlegung von Create, Update, Delete sowie Actions

4. **Handler Klasse**
   - Implementierung der Geschäftslogik
   - Determinations, Validations, Actions und Feature Control

5. **Service Definition & Service Binding**
   - Bereitstellung der Anwendung als **OData V4 Service**

6. **Fiori Elements UI**
   - List Report und Object Page
   - Value Help, Workflow-Aktionen und Statussteuerung

### Prozessfluss

**Tabelle → CDS Views → Behavior Definition → Handler Klasse → OData V4 → Fiori Elements UI**
