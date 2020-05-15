# Web Technology: Implementation & Security - Beroepsproduct

**Ontwikkel je mee aan dit project**? Zie de [workflow en richtlijnen](/.github/CONTRIBUTING.md).

## Inleiding

Dit is een startpunt voor je uitwerking van het beroepsproduct, een website gebaseerd op PHP en SQL Server. Dit project gaat uit van [Visual Studio Code](https://code.visualstudio.com/docs/getstarted/userinterface).

## Stappenplan voor start

Het is belangrijk dat je deze stappen exact in deze volgorde uitvoert om te kunnen beginnen met programmeren.

### 0. Vereisten

- Installeer [Visual Studio Code](https://code.visualstudio.com/).
- Installeer Docker. Dit project is getest met de variant [Docker Desktop](https://www.docker.com/products/docker-desktop).

### 1. GitHub: Haal een kopie van dit project binnen

Dat kan op allerlei manieren. De gemakkelijkste is om het project als een ZIP-archief te downloaden.

Zie: [_Cloning a repository using the command line_](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository#cloning-a-repository-using-the-command-line), alleen stap 3.

### 2. Visual Studio Code: open de workspace

Open het bestand [`/webapplicatie.code-workspace`](/webapplicatie.code-workspace) als workspace.
Zie: [_Opening workspace files_](https://code.visualstudio.com/docs/editor/multi-root-workspaces#_opening-workspace-files).

### 3. Visual Studio Code: open een nieuw venster **voor SQL Server 2019**

Via de menubalk bovenaan: _File_ > _New Window_.

N.B.: Dit venster is en blijft specifiek om te ontwikkelen aan of te werken met SQL Server 2019.

### 4. Browser: Download de database dump

Download de [Adventure Works 2017](https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15) database dump vanaf https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorks2017.bak naar de huidige map `rdbms/`. Sla het bestand op onder de naam `AdventureWorks2017.bak`.

### 5. Visual Studio Code: open de folder `rdbms` in het venster voor SQL Server 2019

Via de menubalk bovenaan: _File_ > _Open..._.
Select de map `rdbms`, dus niet een bestand erbinnen.

### 6. Visual Studio Code: activeer de dev container voor SQL Server 2019

Wacht rustig af tot Visual Studio Code in de blauwe balk onderaan geen activiteit meer vertoont. Dit kan de eerste keer tot wel een kwartier duren, afhankelijk van hoe snel je internetverbinding en computer is.

Op een gegeven moment krijg je de vraag of je de dev container binnen deze map wilt activeren. Reageer met _Yes_.

### 7. Visual Studio Code: open een nieuw venster **voor PHP**

Via de menubalk bovenaan: _File_ > _New Window_.

### 8. Visual Studio Code: open de folder `webserver` in het venster voor PHP

Via de menubalk bovenaan: _File_ > _Open..._. Selecteer de map `webserver`, dus niet een bestand erbinnen.

### 9. Visual Studio Code: activeer de dev container voor PHP

Neem ook hier de inleidende opmerking serieus bij de eerdere stap _... activeer de dev container voor SQL Server 2019_.

Op een gegeven moment krijg je de vraag of je de dev container binnen deze map wilt activeren. Reageer met _Yes_.

### 10. Browser: bezoek nu de website op http://127.0.0.1/

In de huidige versie van dit template moet je even wachten tot de databasebackup is hersteld.

## Vraag en antwoord

### Hoe kan ik dingen uitproberen en uitzoeken aan de database buiten PHP om?

In de dev container [rdbms](/rdbms/) staat de [SQL Server-extensie voor Visual Studio Code](https://docs.microsoft.com/en-us/sql/visual-studio-code/sql-server-develop-use-vscode?view=sql-server-ver15) standaard geïnstalleerd.

Gebruikt https://www.php.net/manual/en/features.commandline.webserver.php
