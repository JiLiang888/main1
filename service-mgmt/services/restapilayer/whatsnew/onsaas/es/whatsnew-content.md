### VMware NSX-T Manager 
#### Aviso de desuso 
* VMware NSX Data Center for vSphere (NSX-V) como origen de datos quedará obsoleto en futuras versiones. 
* Los siguientes servicios se verán afectados después del desuso:
    * **Adición del origen de datos:** No podrá agregar NSX-V como origen de datos.  
    * **Recopilación de datos:** La recopilación de datos se detendrá y se deshabilitará para los orígenes de datos de NSX-V existentes. 
    * **Métricas y flujos:** Los flujos y las métricas asociadas se eliminarán según el período de retención. 
* **Acción requerida:** Migre las instancias de NSX-V a VMware NSX-T y agregue VMware NSX-T instancias como orígenes de datos en VMware Aria Operations for Networks. 

&nbsp;
&nbsp;
### Garantía y verificación de red
* Organice automáticamente toda la asignación de red o un conjunto de grupos seleccionados dentro de la asignación de red. Cuando restablezca el mapa, el diseño se ajustará automáticamente para que se ajuste mejor a la pantalla. 
![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* Seleccione en masa varios dispositivos en la asignación de red y cree grupos fácilmente. También puede seleccionar varios dispositivos y arrastrarlos juntos a una nueva ubicación en la asignación de red. 
* Cree grupos mediante la dirección IP, el rango de IP, la subred y la búsqueda personalizada. Los orígenes de datos recién agregados que coinciden con los criterios de búsqueda se incluyen automáticamente en los grupos relevantes. 
![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* Obtenga alertas generadas por el sistema si alguna intención definida anteriormente no es válida. También puede modificar las intenciones para que coincidan con el escenario actual. 
![](data:image/png;base64,#IMAGEBASE64_intent.png)
* Realice una búsqueda de ruta de acceso de asignación de red con entidades físicas y virtuales en las que el recuento de reglas de red y el recuento de entidades físicas se encuentren dentro de sus respectivos límites.  
* Las validaciones de intención ahora son independientes de la asignación de red si se cumplen los límites descritos anteriormente. 
* Los hosts VMware ESXi ahora se agrupan automáticamente en Asignación de red en función de sus respectivos clústeres de VMware vCenter. 
![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* Cree varios grupos en Asignación de red mediante la opción de importación de CSV a través de la interfaz de línea de comandos.  
![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### Mejoras de la plataforma 
* VMware Aria Operations for Networks admite TLS versión 1.3. 
* Ahora se admite la coexistencia de la suscripción universal de CPU y por núcleo universal. Puede adquirir la suscripción Per Core Universal para la expansión mientras la suscripción CPU Universal sigue activa. El uso se muestra en términos de núcleos.   
* Ahora puede configurar nombres de host para la plataforma y los recopiladores mediante la interfaz de línea de comandos. Estos nombres de host se muestran en la página Infraestructura y soporte, los resultados de búsqueda, las alertas y la página de entidades. 
![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* El cuerpo de captura de SNMP en las alertas tiene campos adicionales de entidad de problema y administrador para mejorar el tiempo medio de reparación (Mean Time To Repair, MTTR). 

&nbsp;
&nbsp;
###  
* Agregue dispositivos físicos configurados con algoritmos de cifrado más seguros para las conexiones SSH como orígenes de datos administrados. Para obtener más información sobre los algoritmos de cifrado compatibles, consulte [ Algoritmos de cifrado y cifrado](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* Ahora puede actualizar en masa las credenciales de SNMP para orígenes de datos de terceros. 
![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* Ahora puede exportar los dispositivos detectados como un archivo CSV. 
![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* Ahora puede importar dispositivos desde un archivo CSV para agregarlos como orígenes de datos. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### Detección de aplicaciones basada en flujos 
* Ahora puede cargar un archivo CSV que utiliza la detección de aplicaciones basadas en flujos (FBAD) para mejorar la detección de aplicaciones. 
    * Utilice la exportación de CSV desde una base de datos de administración de contenido (Content Management Database, CMDB) existente y cargue ese archivo CSV para agregar definiciones de aplicaciones preexistentes y acelerar el proceso de detección de aplicaciones. 
    * Al cargar un archivo CSV para detectar aplicaciones, los nombres de las aplicaciones del archivo CSV se utilizan para nombrar las aplicaciones y los niveles. 
    * Antes de guardar la aplicación, puede modificar sus miembros, niveles y nombre. 
    * Las aplicaciones creadas con la carga de CSV se supervisan en busca de actualizaciones y se muestran en el panel de control de aplicaciones para su aprobación. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* La detección de aplicaciones basada en flujos ahora tiene en cuenta los rangos de puertos dinámicos al agrupar máquinas virtuales en un nivel.  

&nbsp;
&nbsp;
### Paneles de control personalizados
* Nuevos widgets disponibles en la biblioteca de widgets, como principales comunicadores, información de flujo, widgets de aplicaciones, etc.
* El usuario ahora podrá editar los nombres del título del widget.