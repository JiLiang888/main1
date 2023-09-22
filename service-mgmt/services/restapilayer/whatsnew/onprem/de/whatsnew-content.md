### VMware NSX-T Manager 
#### Hinweis zu veralteten 
* VMware NSX Data Center for vSphere (NSX-V) als Datenquelle wird in zukünftigen Versionen nicht mehr unterstützt. 
* Die folgenden Dienste werden beeinträchtigt, nachdem sie veraltet sind:
    * **Hinzufügen einer Datenquelle:** Sie können NSX-V nicht als Datenquelle hinzufügen.  
    * **Datenerfassung:** Die Datenerfassung wird für vorhandene NSX-V-Datenquellen beendet und deaktiviert. 
    * **Metriken und Flows:** Zugeordnete Metriken und Flows werden gemäß dem Aufbewahrungszeitraum gelöscht. 
* **Aktion erforderlich:** Migrieren Sie Ihre NSX-V-Instanzen zu VMware NSX-T und fügen Sie VMware NSX-T-Instanzen als Datenquellen in VMware Aria Operations for Networks hinzu. 

&nbsp;
&nbsp;
### Netzwerksicherung und -überprüfung
* Ordnen Sie Ihre gesamte Netzwerkzuordnung oder eine Gruppe ausgewählter Gruppen innerhalb der Netzwerkzuordnung automatisch an. Wenn Sie die Karte zurücksetzen, wird das Layout automatisch so angepasst, dass es dem Bildschirm am besten entspricht. 
![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* Wählen Sie mehrere Geräte in der Netzwerkzuordnung massenhaft aus und erstellen Sie mühelos Gruppen. Sie können auch mehrere Geräte auswählen und sie an eine neue Position in der Netzwerkzuordnung ziehen. 
* Erstellen Sie Gruppen mithilfe der IP-Adresse, des IP-Bereichs, des Subnetzes und der benutzerdefinierten Suche. Neu hinzugefügte Datenquellen, die den Suchkriterien entsprechen, werden automatisch in die relevanten Gruppen aufgenommen. 
![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* Rufen Sie vom System generierte Warnungen ab, wenn zuvor definierte Absichten ungültig sind. Sie können die Absichten auch so ändern, dass sie ihrem aktuellen Szenario entsprechen. 
![](data:image/png;base64,#IMAGEBASE64_intent.png)
* Führen Sie eine Netzwerkzuordnungspfadsuche mit physischen und virtuellen Einheiten durch, wobei die Gesamtanzahl der Netzwerkregeln und die Anzahl der physischen Einheiten innerhalb ihrer jeweiligen Grenzwerte liegen.  
* Absichtsvalidierungen sind jetzt unabhängig von der Netzwerkzuordnung, wenn die zuvor beschriebenen Grenzwerte erreicht werden. 
* VMware ESXi Hosts werden jetzt automatisch in der Netzwerkzuordnung basierend auf ihren jeweiligen VMware vCenter Clustern gruppiert. 
![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* Erstellen Sie mehrere Gruppen in der Netzwerkzuordnung mithilfe der CSV-Importoption über die Befehlszeilenschnittstelle.  
![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### Verbesserungen bei der Plattform 
* VMware Aria Operations for Networks unterstützt TLS Version 1.3. 
* Die Koexistenz von "CPU Universal" und "Universal pro Kern" wird jetzt unterstützt. Sie können ein Universal-Abonnement pro Kern zur Erweiterung erwerben, während Ihr CPU Universal-Abonnement noch aktiv ist. Die Nutzung wird in Bezug auf die Kerne angezeigt.   
* Sie können jetzt Hostnamen für Plattform und Collectors über die Befehlszeilenschnittstelle konfigurieren. Diese Hostnamen werden auf der Seite "Infrastruktur und Support", auf den Suchergebnissen, auf den Warnungen und auf der Seite "Einheit" angezeigt. 
![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* Der SNMP-Trap-Text in Warnungen enthält zusätzliche Felder mit Problemeinheit und Manager, um die mittlere Reparaturzeit (MTTR) zu verbessern. 

&nbsp;
&nbsp;
###  
* Fügen Sie physische Geräte hinzu, die mit stärkeren Verschlüsselungsalgorithmen für SSH-Verbindungen als verwaltete Datenquellen konfiguriert sind. Weitere Informationen zu den unterstützten Verschlüsselungsalgorithmen finden Sie unter [Verschlüsselungsalgorithmen und Verschlüsselungen](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* Sie können jetzt SNMP-Anmeldedaten für Datenquellen von Drittanbietern massenweise aktualisieren. 
![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* Sie können jetzt erkannte Geräte als CSV-Datei exportieren. 
![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* Sie können jetzt Geräte aus einer CSV-Datei importieren, um sie als Datenquellen hinzuzufügen. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### Flow-basierte Anwendungserkennung 
* Sie können jetzt eine CSV-Datei hochladen, die von der Flow-basierten Anwendungserkennung (FBAD) verwendet wird, um die Erkennung von Anwendungen zu verbessern. 
    * Verwenden Sie den CSV-Export aus einer vorhandenen Inhaltsverwaltungsdatenbank (CMDB) und laden Sie diese CSV-Datei hoch, um bereits vorhandene Anwendungsdefinitionen hinzuzufügen und die Anwendungserkennung zu beschleunigen. 
    * Wenn Sie eine CSV-Datei hochladen, um Anwendungen zu erkennen, werden die Anwendungsnamen aus der CSV-Datei verwendet, um die Anwendungen und Ebenen zu benennen. 
    * Vor dem Speichern der Anwendung können Sie deren Mitglieder, Ebenen und Namen ändern. 
    * Anwendungen, die mithilfe des CSV-Uploads erstellt wurden, werden auf Updates überwacht und im Anwendungs-Dashboard zur Genehmigung angezeigt. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* Die Flow-basierte Anwendungserkennung berücksichtigt jetzt dynamische Portbereiche beim Gruppieren von VMs in einer Ebene.  

&nbsp;
&nbsp;
### Benutzerdefinierte Dashboards
* Neue Widgets, die in der Widget-Bibliothek verfügbar sind, wie z. B. top Talker, Flow Insights, Anwendungs-Widgets usw.
* Der Benutzer kann jetzt die Namen des Widget-Titels bearbeiten.