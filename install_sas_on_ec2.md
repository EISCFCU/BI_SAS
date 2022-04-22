# SAS EG on AWS EC2

適用Learner Lab

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

25.成功遠端桌面
![image](https://user-images.githubusercontent.com/103306835/164401007-ab1c527c-8936-4fce-b824-ef85deee2d9e.png)


# 權限設定

1.點選開始列中的Server Manager

![image](https://user-images.githubusercontent.com/103306835/164401897-02e3f74a-1227-4a0e-bf70-450e1cd5d4a3.png)

2.點選Local Server

![image](https://user-images.githubusercontent.com/103306835/164402416-415bb716-95a1-4047-971c-164589b2e752.png)

3.將IE Enhanced Security Configuration切換為OFF

![image](https://user-images.githubusercontent.com/103306835/164402989-0f47d0df-1ee1-44ec-8cf5-18ffc1358bcf.png)
![image](https://user-images.githubusercontent.com/103306835/164403104-5281e7d1-2f5c-4e90-b998-d52948a149e8.png)
![image](https://user-images.githubusercontent.com/103306835/164403206-01f36f1f-dd9a-439b-a8b2-f9ebe310cf2e.png)
![image](https://user-images.githubusercontent.com/103306835/164403330-e1c93939-8cf5-43a1-94db-ffe40236cb27.png)

4.開啟IE
![image](https://user-images.githubusercontent.com/103306835/164403585-be7cf3f1-2ac8-4b1c-8ffe-092035282875.png)

5.網址列輸入https://www.sas.com/zh_tw/software/on-demand-for-academics.html



# 安裝SAS EG 8.2

1.點選[Access Now]

![image](https://user-images.githubusercontent.com/103306835/164397262-f1d7bbcd-8249-4ae4-8871-1aa46a117b98.png)

2.輸入帳號密碼 並Sign In

![image](https://user-images.githubusercontent.com/103306835/164397357-4d513e9c-ead5-495f-b0f9-82a46f176362.png)

3.點選[Enrollments]頁籤

![image](https://user-images.githubusercontent.com/103306835/164397461-43cbcf23-61ad-4257-ae71-078b5a1ce6de.png)

4.點選[+enroll in a course]

![image](https://user-images.githubusercontent.com/103306835/164397576-8560bbd3-825c-4130-af88-c35d9733f6a0.png)

5.輸入Course Code 並點選Continue
Course Code：3ddbdc4f-07d8-48ec-910e-549f9b9a22bd

![image](https://user-images.githubusercontent.com/103306835/164397783-a13240fe-552b-4f1b-8922-79f992c0dea9.png)

6.點選[Applications]

![image](https://user-images.githubusercontent.com/103306835/164397933-a9804336-585c-4fa1-9053-6bbc806c7639.png)

7.點選[SAS Enterprise Guide]

![image](https://user-images.githubusercontent.com/103306835/164398031-88aba4c4-4cf0-4bfc-ad0e-e4e38cfeedcf.png)

8.點選[eguideoda_signed.exe]

![image](https://user-images.githubusercontent.com/103306835/164398131-1262378a-1ff4-41ea-829a-acf3f175d1f9.png)

9.點選[Install]

![image](https://user-images.githubusercontent.com/103306835/164398247-9430a5c2-fa07-46b1-84da-7d4f03dc72e7.png)

10.等待安裝

![image](https://user-images.githubusercontent.com/103306835/164398359-72871750-ed45-40df-be60-01b1c522e1b0.png)

11.等待安裝

![image](https://user-images.githubusercontent.com/103306835/164398493-7cf6b2f4-de99-41e0-bb5b-b7e5229e882e.png)

12.選擇[繁體中文] 並點選[確定]

![image](https://user-images.githubusercontent.com/103306835/164398581-0ad1ce40-fdcf-40d4-90a0-c8a60e94435c.png)

13.查看電腦作業系統位元 並選擇安裝SAS EG模式(64 或32位元)

![image](https://user-images.githubusercontent.com/103306835/164398735-7fc96f5e-5e1c-4153-bafc-d1eecba29427.png)

14.選擇[繁體中文] 並點選[下一步]

![image](https://user-images.githubusercontent.com/103306835/164398826-82ef8f32-51c0-4b23-b58d-384e061c1bbf.png)

15.等待部署

![image](https://user-images.githubusercontent.com/103306835/164398939-3aaa8f28-701e-4fa3-af29-c8ddf4e98875.png)

16.點選[安裝] 會出現下方開始部署的示意圖

![image](https://user-images.githubusercontent.com/103306835/164399038-13260767-99b3-49d9-afa0-68d2c10830d4.png)

17.等待安裝

![image](https://user-images.githubusercontent.com/103306835/164399142-e7a58fac-00c0-46a3-b1d9-6e32fda90086.png)

18.點選[下一步]

![image](https://user-images.githubusercontent.com/103306835/164399256-b5487a7e-9b4e-4bfa-acab-9d29320c0fb7.png)

19.點選[完成]

![image](https://user-images.githubusercontent.com/103306835/164399343-3390777e-8984-4629-9817-800c430ce76d.png)

# SAS Enterprise Guide 8.2 OnDemand for Academics登入

1.開啟SAS Enterprise Guide 8.2 Ondemand for Academic

![image](https://user-images.githubusercontent.com/103306835/164399545-b1d5a1e2-00f7-4009-944d-dcd8d9d6e8ac.png)

2.輸入SAS OnDemand for Academics帳密

![image](https://user-images.githubusercontent.com/103306835/164399665-cc57f430-ab29-4077-8d46-5d40def4cd18.png)

3.驗證中

![image](https://user-images.githubusercontent.com/103306835/164399748-14c4a6e1-2773-42ed-9a5e-e4c837005777.png)

4.可使用SAS Enterprise Guide

![image](https://user-images.githubusercontent.com/103306835/164399849-ad9997c7-036f-4ef1-9106-db601a27a4f0.png)

