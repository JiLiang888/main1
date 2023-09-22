### VMware NSX-T Manager 
#### 弃用通知 
* VMware NSX Data Center for vSphere （NSX-V） 作为数据源将在未来版本中弃用。 
* 弃用后，以下服务将受到影响：
    * **添加数据源：** 您将无法将 NSX-V 添加为数据源。  
    * **数据收集：** 将停止并禁用现有 NSX-V 数据源的数据收集。 
    * **衡量指标和流：** 将根据保留期删除关联的衡量指标和流。 
* **需要操作：** 将 NSX-V 实例迁移到VMware NSX-T，并在 VMware Aria Operations for Networks 中添加 VMware NSX-T 实例作为数据源。 

&nbsp;
&nbsp;
### 网络保证和验证
* 自动排列整个网络映射或网络映射中的一组选定组。重置映射时，将自动调整布局以最符合屏幕要求。![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* 在网络映射上批量选择多个设备，并轻松创建组。您还可以选择多个设备，并将其一起拖动到“网络映射”中的新位置。 
* 使用 IP 地址、IP 范围、子网和自定义搜索创建组。新添加的与搜索条件匹配的数据源将自动包含在相关组中。![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* 如果任何先前定义的意向无效，则获取系统生成的警示。您还可以修改意向以匹配当前方案。![](data:image/png;base64,#IMAGEBASE64_intent.png)
* 对网络规则总数和物理实体总数在各自限制内的物理实体和虚拟实体执行网络映射路径搜索。  
* 如果满足之前描述的限制，意向验证现在独立于网络映射。 
* VMware ESXi主机现在根据主机各自的VMware vCenter集群自动分组到网络映射中。![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* 通过命令行界面使用 CSV 导入选项在网络映射中创建多个组。![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### 平台增强功能 
* VMware Aria Operations for Networks 支持 TLS 版本 1.3。 
* 现在支持 CPU 通用和每内核通用订阅共存。您可以在 CPU 通用订阅仍处于活动状态时购买每内核通用订阅以进行扩展。使用情况以内核数显示。   
* 现在，您可以使用命令行界面为平台和收集器配置主机名。这些主机名显示在“基础架构和支持”页面、搜索结果、警示和实体页面上。![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* 警示中的 SNMP 陷阱正文具有问题实体和管理器的其他字段，可缩短平均修复时间 （MTTR）。 

&nbsp;
&nbsp;
###  
* 将配置了更强密码算法的物理设备作为受管数据源进行 SSH 连接。有关支持的密码算法的更多详细信息，请参见 [Encryption Algorithms and Ciphers ](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* 现在，您可以批量更新第三方数据源的 SNMP 凭据。![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* 您现在可以将发现的设备导出为 CSV 文件。![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* 现在，您可以从 CSV 文件导入设备，以将其添加为数据源。![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### 基于流的应用程序发现 
* 现在，您可以上载 CSV 文件，基于流的应用程序发现 （FBAD） 使用该文件来改进应用程序的发现。 
    * 使用从现有内容管理数据库 （CMDB） 导出 CSV 并上载该 CSV 文件，以添加预先存在的应用程序定义并加速应用程序发现过程。 
    * 上载 CSV 文件以发现应用程序时，CSV 文件中的应用程序名称将用于命名应用程序和层。 
    * 在保存应用程序之前，您可以修改其成员、层和名称。 
    * 使用 CSV 上载创建的应用程序将监控更新，并显示在应用程序仪表板上以供审批。![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* 现在，基于流的应用程序发现在将虚拟机分组到层时会考虑动态端口范围。  

&nbsp;
&nbsp;
### 自定义仪表板
* 小组件库中提供的新小组件，如“通信最多者”、“流见解”、“应用程序小组件”等。
* 用户现在可以编辑小组件标题的名称。