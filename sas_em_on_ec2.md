# SAS EM on AWS EC2

適用Learner Lab

# SAS 帳號註冊(已有帳號者請略過此步驟)

1.搜尋SAS Ondemand for academics

連結：https://www.sas.com/zh_tw/software/on-demand-for-academics.html

![image](https://user-images.githubusercontent.com/103306835/163938096-8fdface4-3ade-43ee-8f6e-17a24c82a783.png)

2.點選[Access Now]

![image](https://user-images.githubusercontent.com/103306835/163938115-0e51ec7b-2a0f-4684-9677-d23f414c723d.png)

3.點選Sign In

![image](https://user-images.githubusercontent.com/103306835/164383890-12f9c332-f121-4cda-a82a-5c3b146a0467.png)

4.點選[Create Profile]

![image](https://user-images.githubusercontent.com/103306835/164383976-55f4060c-ef08-46d2-88fd-7d714dd1ead3.png)

5.輸入資料

![image](https://user-images.githubusercontent.com/103306835/164384072-f4b433d4-a30d-4be0-887a-8f52c49e6752.png)
![image](https://user-images.githubusercontent.com/103306835/164384120-6c520f5e-f7b5-44b6-be71-d86960e6812e.png)

6.點選[建立個人認證帳戶]

![image](https://user-images.githubusercontent.com/103306835/164384262-832b3e21-3989-438b-9e58-a545a512c90b.png)

7.完成建立帳戶

![image](https://user-images.githubusercontent.com/103306835/164384311-04359ad9-7811-459b-bd2b-73c87caa3e9e.png)

8.至註冊信箱收信

![image](https://user-images.githubusercontent.com/103306835/164384402-f9d44b82-7380-4041-b170-08b1f7742fb8.png)

9.點選[啟動您的SAS個人資料文件]

![image](https://user-images.githubusercontent.com/103306835/164384444-5e7a9580-4d9c-417d-9051-59b75e0ee098.png)

10.點選[設置密碼]

![image](https://user-images.githubusercontent.com/103306835/164384478-ac772822-6220-432d-b4b2-3a79c45b6fb7.png)

11.點選[繼續]

![image](https://user-images.githubusercontent.com/103306835/164384531-194c0f1b-c3d5-485c-a130-7604462a1273.png)

12.點選[登入]

![image](https://user-images.githubusercontent.com/103306835/164384575-403df8f9-aa2b-477a-8600-3467349191cd.png)

13.點選[登入]

![image](https://user-images.githubusercontent.com/103306835/164384608-1140bc9a-6b1f-4015-90bf-c46d8f2d0b6b.png)

14.輸入使用者名稱

![image](https://user-images.githubusercontent.com/103306835/164384718-7e4eff44-1244-43ea-b31d-689a327ab413.png)

15.點選[下一步]

![image](https://user-images.githubusercontent.com/103306835/164384762-1d32d3d1-aeef-4f89-9dbb-b631cfedf5e0.png)

# SAS ON EC2

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

14.勾選SASEM的虛擬機

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
# for mac 遠端桌面使用(
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



# 安裝SAS EM(此時在遠端桌面環境)

1.點選[Access Now]

![image](https://user-images.githubusercontent.com/103306835/164397262-f1d7bbcd-8249-4ae4-8871-1aa46a117b98.png)

2.輸入帳號密碼 並Sign In

![image](https://user-images.githubusercontent.com/103306835/164397357-4d513e9c-ead5-495f-b0f9-82a46f176362.png)


3.點選[SAS Enterprise Miner]

![image](https://user-images.githubusercontent.com/103306835/172974327-016d9a20-2799-4fac-94a6-aaa209347c4e.png)


4.點選[Configuration]

![image](https://user-images.githubusercontent.com/103306835/172974335-37c0592c-441f-46ef-8176-db24a10cf2b9.png)

5.點選[Here]

![image](https://user-images.githubusercontent.com/103306835/172974371-27597adb-6c15-49ee-a7dd-6d05ac992520.png)

6.點選[JRE for consumers]

![image](https://user-images.githubusercontent.com/103306835/172974542-926b833a-3793-4a4f-93a2-41c5d650820c.png)

7.點選[下載JAVA]

![image](https://user-images.githubusercontent.com/103306835/172974665-4b618971-d456-4f51-b509-3d92aa0a96fc.png)

8.點選[Run]

![image](https://user-images.githubusercontent.com/103306835/172974783-42ea8b98-9673-4a5f-bea4-8d428c9e5ffc.png)

9.點選[Install]

![image](https://user-images.githubusercontent.com/103306835/172974842-21814050-3f7b-4c1c-9ecf-9a57f4a3890d.png)


10.等待安裝

![image](https://user-images.githubusercontent.com/103306835/172974922-085a1860-f6b4-41f1-97c7-dc86b7e0bfee.png)

11.點選[Close]

![image](https://user-images.githubusercontent.com/103306835/172975003-b312dd5f-94f0-4e56-bf5c-c9b77f5478fe.png)

12.點選[Main.jnlp]進行安裝

![image](https://user-images.githubusercontent.com/103306835/172975269-3e58ef0d-db92-4043-bc32-fac1039c50e5.png)

13.等待安裝

14.搜尋[Command Prompt]

![image](https://user-images.githubusercontent.com/103306835/172975351-d0767e4b-c64c-4f34-b714-1aaeb3d84930.png)

15.輸入javaws -viewer

![image](https://user-images.githubusercontent.com/103306835/172975519-a14e8b9a-e7bd-41d2-a67e-1e21a1b9a38d.png)

16.點選SAS EM

![image](https://user-images.githubusercontent.com/103306835/172975572-67e0c3b0-360e-4ae8-afa8-6520c5ece627.png)

17.點選[Run]

![image](https://user-images.githubusercontent.com/103306835/172975613-8d608676-4f3c-4e19-a84a-02f8bd9242c6.png)

18.成功開啟SAS EM

![image](https://user-images.githubusercontent.com/103306835/172975679-9f43b3eb-c7e9-4724-b858-121570229a49.png)


# SAS Enterprise Miner 15.1 OnDemand for Academics檔案上傳

1.點選SAS Studio

![image](https://user-images.githubusercontent.com/103306835/172975827-64a54c44-4522-4882-8146-ee78fed82afd.png)

2.點選檔案

![image](https://user-images.githubusercontent.com/103306835/172975867-53fb4ed6-0b8d-476b-8e67-3d3e503f6c1f.png)

3.點選[檔案上傳]

![image](https://user-images.githubusercontent.com/103306835/172975974-5146c4b0-5c4e-4352-b288-a3c672524ecf.png)

4.點選[選擇檔案]

![image](https://user-images.githubusercontent.com/103306835/172975998-162b2368-7ef8-42d8-8fd6-5723e76304a5.png)

5.點選[上傳]

![image](https://user-images.githubusercontent.com/103306835/172976140-251c5fe2-928d-44d2-b6fb-39260fc93bb2.png)

# SAS Enterprise Miner 15.1如何找到上傳檔案

![image](https://user-images.githubusercontent.com/103306835/172976389-290940fd-4e43-4c6a-890e-aafcd0cde211.png)
