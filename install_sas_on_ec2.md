# SAS EG on AWS EC2

1.搜尋EC2
![image](https://user-images.githubusercontent.com/103306835/164387469-93348892-c50e-48b3-9506-ff838b90ec16.png)

2.點選[EC2]

![image](https://user-images.githubusercontent.com/103306835/164387927-0710faaf-5863-46b1-b8bf-79a665e3e279.png)

3.點選[Instances執行個體]

![image](https://user-images.githubusercontent.com/103306835/164388118-c08773fa-50b6-47d7-836f-d0a466ccb16e.png)

3.點選[Launch Instances啟動新執行個體]

![image](https://user-images.githubusercontent.com/103306835/164388254-909a3924-9b94-48a7-8860-cd4e49291b9b.png)

4.輸入名稱(可以自訂)

![image](https://user-images.githubusercontent.com/103306835/164388766-53a08a18-540c-4bfd-95c7-2e60faa9dd36.png)

5.作業系統點選Windows

![image](https://user-images.githubusercontent.com/103306835/164388974-edfa53b8-a91d-4f9c-a86d-e676e78c01d4.png)

6.點選[確認變更]

![image](https://user-images.githubusercontent.com/103306835/164389124-34cfd482-59bb-44d5-ab33-da2da0225dc8.png)

7.作業系統變更成Windows Server

![image](https://user-images.githubusercontent.com/103306835/164389493-59c9dbf8-9658-4332-87ab-e1e4ba026808.png)

8.選擇金鑰名稱：vockey

![image](https://user-images.githubusercontent.com/103306835/164389888-b642f0c3-6663-4a48-b7e8-233bf882f1d6.png)

9.勾選允許RDP流量，來自0.0.0.0/0

![image](https://user-images.githubusercontent.com/103306835/164390423-e7212c21-e1e5-45aa-bd5c-37ad56475a53.png)

10.點選[啟動執行個體]

![image](https://user-images.githubusercontent.com/103306835/164390673-1736819b-6cba-4a4a-8721-ced8f6191fb6.png)

11.點選[檢視所有執行個體]

![image](https://user-images.githubusercontent.com/103306835/164390839-8abf5825-b127-4503-920a-ee3eb3b7de1a.png)

12.等待狀態檢查到2/2

![image](https://user-images.githubusercontent.com/103306835/164391303-c2890f20-2cde-4718-aba9-48b613294076.png)
![image](https://user-images.githubusercontent.com/103306835/164391391-0b4a2d04-ebf7-4c3c-9279-3e78e89a78d6.png)

13.點選[AWS Details]

![image](https://user-images.githubusercontent.com/103306835/164391573-78572fa3-017c-43e4-860f-30594bca7cff.png)

13.點選[Download PEM]

![image](https://user-images.githubusercontent.com/103306835/164391767-a8cffb4c-93af-42b6-a3ac-ca1be24576cf.png)

14.勾選SASEG的虛擬機

![image](https://user-images.githubusercontent.com/103306835/164392013-c48ed38a-dab5-4530-a43f-dcfe63add429.png)

15.點選[連線]

![image](https://user-images.githubusercontent.com/103306835/164392085-579c0e6a-bc66-470d-b631-5df848ef63e2.png)

16.點選[RDP用戶端]

![image](https://user-images.githubusercontent.com/103306835/164392224-41679bf1-23d5-432d-a7d1-65e343651cc9.png)

17.點選[取得密碼]

![image](https://user-images.githubusercontent.com/103306835/164392353-411953ca-45f1-42a8-b495-d6c65a679991.png)

18.點選[Browse]

![image](https://user-images.githubusercontent.com/103306835/164392542-1f917b99-3461-4fb2-9915-7aa940b5f172.png)

19.將金鑰匯入

![image](https://user-images.githubusercontent.com/103306835/164392948-2d4c9731-aff9-426b-85f0-7da9175f64f2.png)

20.點選[解密密碼]

![image](https://user-images.githubusercontent.com/103306835/164393055-856697ca-6023-4ace-8458-f6c4c1835941.png)

21.下載Microsoft Remote Desktop Beta
https://install.appcenter.ms/orgs/rdmacios-k2vy/apps/microsoft-remote-desktop-for-mac/distribution_groups/all-users-of-microsoft-remote-desktop-for-mac

22.在 [連接中心] 中選取 + ，然後選取 [ 新增遠端資源]。

23.輸入遠端資源的資訊：

摘要 URL-RD Web 存取伺服器的 URL。 您也可以在此欄位中輸入您的公司電子郵件帳戶，如此會告訴用戶端搜尋與您電子郵件地址相關聯的 RD Web 存取伺服器。

使用者名稱-您要連線的 RD Web 存取伺服器所要使用的使用者名稱。

密碼-您要連線的 RD Web 存取伺服器所要使用的密碼。

24.選取[儲存]。

