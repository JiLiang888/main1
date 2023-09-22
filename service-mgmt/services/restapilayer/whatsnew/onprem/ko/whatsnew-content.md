### VMware NSX-T Manager 
#### 사용 중단 알림 
* 데이터 소스로 VMware NSX Data Center for vSphere(NSX-V)는 향후 릴리스에서 더 이상 사용되지 않습니다. 
* 다음 서비스는 사용 중단 후 영향을 받게 됩니다.
    * **데이터 소스 추가:** NSX-V를 데이터 소스로 추가할 수 없습니다.  
    * **데이터 수집:** 기존 NSX-V 데이터 소스에 대해 데이터 수집이 중지되고 사용되지 않도록 설정됩니다. 
    * **메트릭 및 흐름:** 연결된 메트릭 및 흐름은 보존 기간에 따라 삭제됩니다. 
* **작업 필요:** NSX-V 인스턴스를 VMware NSX-T 마이그레이션하고 VMware Aria Operations for Networks VMware NSX-T 인스턴스를 데이터 소스로 추가합니다. 

&nbsp;
&nbsp;
### 네트워크 보증 및 검증
* 전체 네트워크 맵 또는 네트워크 맵 내에서 선택한 그룹 집합을 자동으로 정렬합니다. 맵을 재설정하면 화면에 가장 잘 맞도록 레이아웃이 자동으로 조정됩니다. 
![](data:image/png;base64,#IMAGEBASE64_auto_arrange.png)
* 네트워크 맵에서 여러 디바이스를 대량으로 선택하고 그룹을 쉽게 생성합니다. 여러 디바이스를 선택하고 함께 네트워크 맵의 새 위치로 끌어서 놓을 수도 있습니다. 
* IP 주소, IP 범위, 서브넷 및 사용자 지정 검색을 사용하여 그룹을 생성합니다. 검색 조건과 일치하는 새로 추가된 데이터 소스는 관련 그룹에 자동으로 포함됩니다. 
![](data:image/png;base64,#IMAGEBASE64_create_group.png)
* 이전에 정의된 의도가 유효하지 않은 경우 시스템 생성 경고를 가져옵니다. 현재 시나리오와 일치하도록 의도를 수정할 수도 있습니다. 
![](data:image/png;base64,#IMAGEBASE64_intent.png)
* 총 네트워크 규칙 수 및 총 물리적 엔티티 수가 해당 제한 내에 있는 물리적 및 가상 엔티티를 사용하여 네트워크 맵 경로 검색을 수행합니다.  
* 이전에 설명한 제한이 충족되면 의도 유효성 검사는 이제 네트워크 맵과 독립적입니다. 
* 이제 VMware ESXi 호스트는 해당하는 VMware vCenter 클러스터를 기반으로 네트워크 맵에서 자동으로 그룹화됩니다. 
![](data:image/png;base64,#IMAGEBASE64_esxi.png)
* 명령줄 인터페이스를 통해 CSV 가져오기 옵션을 사용하여 네트워크 맵에서 여러 그룹을 생성합니다.  
![](data:image/png;base64,#IMAGEBASE64_create_groups_through_cli.png)

&nbsp;
&nbsp;
### 향상된 플랫폼 기능 
* VMware Aria Operations for Networks TLS 버전 1.3을 지원합니다. 
* 이제 CPU 범용 및 코어별 범용 구독의 공동 존재가 지원됩니다. CPU 범용 구독이 여전히 활성 상태인 동안 확장을 위해 코어별 범용 구독을 구매할 수 있습니다. 사용량은 코어 측면에서 표시됩니다.   
* 이제 명령줄 인터페이스를 사용하여 플랫폼 및 수집기 호스트 이름을 구성할 수 있습니다. 이러한 호스트 이름은 인프라 및 지원 페이지, 검색 결과, 경고 및 엔티티 페이지에 표시됩니다. 
![](data:image/png;base64,#IMAGEBASE64_hostnames.png)
* 경고의 SNMP 트랩 본문에는 MTTR(평균 복구 시간)을 개선하기 위한 문제 엔티티 및 관리자의 추가 필드가 있습니다. 

&nbsp;
&nbsp;
###  
* SSH 연결에 대해 더 강력한 암호 알고리즘으로 구성된 물리적 디바이스를 관리 데이터 소스로 추가합니다. 지원되는 암호 알고리즘에 대한 자세한 내용은 [Encryption 알고리즘 및 암호](https://docs.vmware.com/en/VMware-Aria-Operations-for-Networks/SaaS/Using-Operations-for-Networks/GUID-02B7DC96-66A6-4CDF-9E3E-E25D4C0A8DEC.html)
* 이제 타사 데이터 소스에 대한 SNMP 자격 증명을 대량으로 업데이트할 수 있습니다. 
![](data:image/png;base64,#IMAGEBASE64_snmp.png)
* 이제 검색된 디바이스를 CSV 파일로 내보낼 수 있습니다. 
![](data:image/png;base64,#IMAGEBASE64_export_csv.png)
* 이제 CSV 파일에서 디바이스를 가져와서 데이터 소스로 추가할 수 있습니다. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv.png)

&nbsp;
&nbsp;
### 흐름 기반 애플리케이션 검색 
* 이제 FBAD(흐름 기반 애플리케이션 검색)에서 사용하는 CSV 파일을 업로드하여 애플리케이션 검색을 개선할 수 있습니다. 
    * 기존 CMDB(컨텐츠 관리 데이터베이스)에서 CSV 내보내기를 사용하고 해당 CSV 파일을 업로드하여 기존 애플리케이션 정의를 추가하고 애플리케이션 검색 프로세스를 가속화합니다. 
    * CSV 파일을 업로드하여 애플리케이션을 검색하면 CSV 파일의 애플리케이션 이름이 애플리케이션 및 계층의 이름을 지정하는 데 사용됩니다. 
    * 애플리케이션을 저장하기 전에 해당 멤버, 계층 및 이름을 수정할 수 있습니다. 
    * CSV 업로드를 사용하여 생성된 애플리케이션은 업데이트를 모니터링하며 승인을 위해 애플리케이션 대시보드에 표시됩니다. 
![](data:image/png;base64,#IMAGEBASE64_upload_csv_fbad.png)
* 흐름 기반 애플리케이션 검색은 이제 VM을 계층으로 그룹화할 때 동적 포트 범위를 고려합니다.  

&nbsp;
&nbsp;
### 사용자 지정 대시보드
* 상위 토커, 흐름 인사이트, 애플리케이션 위젯 등과 같은 위젯 라이브러리에서 사용할 수 있는 새 위젯.
* 이제 사용자가 위젯 제목 이름을 편집할 수 있습니다.