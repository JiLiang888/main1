### VMware NSX-T Manager 
#### Deprecation Notice 
* VMware NSX Data Center for vSphere (NSX-V) as a data source will be deprecated in the future releases. 
* The following services will be impacted after deprecation:
    * **Addition of data source:** You will be unable to add NSX-V as a data source.  
    * **Data collection:** Data collection will be stopped and disabled for existing NSX-V data sources. 
    * **Metrics and Flows:** Associated metrics and flows will be deleted as per the retention period. 
* **Action Required:** Migrate your NSX-V instances to VMware NSX-T and add VMware NSX-T instances as data sources in VMware Aria Operations for Networks. 

&nbsp;
&nbsp;
### Network Assurance and Verification
* Auto-arrange your entire Network Map or a set of selected groups within the Network Map. When you reset the map, the layout is automatically adjusted to best fit the screen. 
![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* Bulk select multiple devices on the Network Map and easily create groups. You can also select multiple devices and drag them together to a new location in the Network Map. 
* Create groups using IP address, IP range, subnet, and custom search. Newly added data sources matching the search criteria are automatically included in the relevant groups. 
![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* Get system generated alerts if any previously defined intents are not valid. You can also modify the intents to match your current scenario. 
![](data:image/png;base64,#IMAGEBASE64_intent.png)
* Perform Network Map path search with physical and virtual entities where the total network rule count and total physical entity count are within their respective limits.  
* Intent validations are now independent of Network Map if the previously described limits are met. 
* VMware ESXi Hosts are now automatically grouped in Network Map based on their respective VMware vCenter clusters. 
![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* Create multiple groups in Network Map using the CSV import option through command line interface.  
![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### Platform Enhancements 
* VMware Aria Operations for Networks supports TLS version 1.3. 
* Co-existence of CPU Universal and Per Core Universal subscription is now supported. You can purchase Per Core Universal subscription for expansion while your CPU Universal subscription is still active. The usage is displayed in terms of cores.   
* You can now configure hostnames for platform and collectors using the command line interface. These hostnames are displayed on the Infrastructure and Support page, search results, alerts, and the entity page. 
![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* SNMP trap body in alerts have additional fields of problem entity and manager to improve the mean time to repair (MTTR). 

&nbsp;
&nbsp;
### Third-party devices 
* Add physical devices configured with stronger cipher algorithms for SSH connections as managed data sources. For more details on the supported cipher algorithms, see [Encryption Algorithms and Ciphers](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* You can now bulk update SNMP credentials for third-party data sources. 
![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* You can now export discovered devices as a CSV file. 
![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* You can now import devices from a CSV file to add them as data sources. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### Flow-based Application Discovery 
* You can now upload a CSV file which is used by Flow-based Application Discovery (FBAD) to improve the discovery of applications. 
    * Use CSV export from an existing Content Management Database (CMDB) and upload that CSV file to add pre-existing application definitions and accelerate the application discovery process. 
    * When you upload a CSV file to discover applications, the application names from the CSV file are used to name the applications and tiers. 
    * Before saving the application, you can modify its members, tiers, and name. 
    * Applications created using the CSV upload are monitored for updates and are shown on the Application Dashboard for approval. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* Flow-based Application Discovery now considers dynamic port ranges when grouping VMs into a tier.  

&nbsp;
&nbsp;
### Custom Dashboards
* New widgets available in the widget library like the Top Talkers, Flow Insights , Application Widgets etc.
* User will now be able to edit the names of the widget title.