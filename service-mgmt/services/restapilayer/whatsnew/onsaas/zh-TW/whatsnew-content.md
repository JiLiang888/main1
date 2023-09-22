### VMware NSX-T Manager 
#### 棄用通知 
* 在未來版本中，做為資料來源的VMware NSX Data Center for vSphere （NSX-V） 將被取代。 
* 下列服務將在棄用後受到影響：
    * **新增資料來源：** 您將無法將 NSX-V 新增為數據源。  
    * **資料收集：** 現有 NSX-V 資料來源的資料收集將停止並停用。 
    * **度量和流量：** 將根據保留期間刪除相關聯的度量和流量。 
* **需要採取動作：** 將 NSX-V 實例移轉至 VMware NSX-T，並在 VMware Aria Operations for Networks 中將VMware NSX-T實例新增為數據源。 

&nbsp;
&nbsp;
### 網路保證與驗證
* 自動排文整個網路對應，或在網路對應內排列一組選取的群組。當您重設地圖時，會自動調整配置以最貼合螢幕。![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* 大量選取網路對應上的多個裝置，並輕鬆建立群組。您也可以選取多個裝置，並將其一起拖曳至 [網路對應] 中的新位置。 
* 使用 IP 位址、IP 範圍、子網和自訂搜尋建立群組。符合搜尋準則的新增資料來源會自動包含在相關群組中。![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* 如果先前定義的任何意圖無效，則取得系統產生的警示。您也可以修改意圖以符合您目前的案例。![](data:image/png;base64,#IMAGEBASE64_intent.png)
* 對實體和虛擬實體執行網路對應路徑搜尋，其中網路規則總計數和實體總計數都在各自的限制內。  
* 如果符合先前說明的限制，則意圖驗證現在獨立于網路對應。 
* VMware ESXi主機現在會根據其各自的VMware vCenter叢集在網路對應中自動分組。![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* 透過命令列介面使用 CSV 匯入選項在網路對應中建立多個群組。![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### 平台增強功能 
* VMware Aria Operations for Networks 支援 TLS 版本 1.3。 
* 現在支援 CPU 通用訂閱與每個核心的通用訂閱並存。當 CPU 通用訂閱仍處於作用中狀態時，您可以購買按核心通用訂閱以進行擴充。會以核心數顯示使用量。   
* 您現在可以使用命令列介面設定平臺和收集器的主機名稱。這些主機名稱會顯示在 [基礎結構和支援] 頁面、搜尋結果、警示和實體頁面上。![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* 警示中的 SNMP 設陷本文具有問題實體和管理程式的其他欄位，可縮短平均修復時間 （MTTR）。 

&nbsp;
&nbsp;
###  
* 將設定了使用增強型加密演算法進行 SSH 連線的實體裝置新增為受管理資料來源。如需有關支援的加密演算法的更多詳細資料，請參閱 [加密演算法 和 加密 ](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* 您現在可以為協力廠商資料來源大量更新 SNMP 認證。![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* 您現在可以將探索到的裝置匯出為 CSV 檔案。![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* 您現在可以從 CSV 檔案匯入裝置，以將其新增為數據源。![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### 以流量為基礎的應用程式探索 
* 您現在可以上傳 CSV 檔案，該檔案由以流量為基礎的應用程式探索 （FBAD） 使用，以改善應用程式的探索。 
    * 使用現有內容管理資料庫 （CMDB） 的 CSV 匯出並上傳該 CSV 檔案，以新增既存的應用程式定義並加速應用程式探索程式。 
    * 上傳 CSV 檔案以探索應用程式時，會使用 CSV 檔案中的應用程式名稱來命名應用程式和層。 
    * 儲存應用程式之前，您可以修改其成員、層和名稱。 
    * 使用 CSV 上傳建立的應用程式會受到監控的更新，並顯示在應用程式儀表板上以供核准。![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* 以流量為基礎的應用程式探索現在會在將虛擬機器分組到階層時考慮動態埠範圍。  

&nbsp;
&nbsp;
### 自訂儀表板
* Widget 程式庫中提供了新的 Widget，例如最高排名通訊者、流量見解、應用程式 Widget 等。
* 使用者現在可以編輯 Widget 標題的名稱。