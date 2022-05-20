# POS資料存儲與分析

# 情境

ABC飲料店是台灣連鎖知名飲料店，累積開店數約500家，自建POS系統已搬遷到雲端資料庫(postgresql)。
業務主管小陳想查看2021年各縣市與營業額的資訊。身為資料分析師的你，請進行簡易的資料分析，並提供主管小林一份簡易統計報表。

# POS資料描述

![image](https://user-images.githubusercontent.com/103306835/169325602-ec1517e8-3087-4909-a1b2-071b50f4bbbb.png)


# 資料存儲與分析步驟

![image](https://user-images.githubusercontent.com/103306835/169325707-d6f6db58-db45-4c1a-8210-1a310a0f8b8a.png)

# 實作架構

![image](https://user-images.githubusercontent.com/103306835/169325768-a607eb00-6f25-4249-8cba-eca54e910c1d.png)

# 使用環境(請先Start Lab)
AWS Academy Learner Lab-Foundation Services

AWS Academy登入連結：https://awsacademy.instructure.com/login/canvas

如何進入Learner Lab，請參考：https://github.com/EISCFCU/ntue_cloud-database/blob/main/Quick%20Lab%230%E9%80%B2%E5%85%A5AWS%20Academy.md

# 使用資源(請先下載)

1.sqlectron：https://sqlectron.github.io/

1-1.下載sqlectron，連結：https://sqlectron.github.io/

1-2.點選GUI

![image](https://user-images.githubusercontent.com/103306835/167972790-e833bc5d-f8e2-4208-8ffc-98ed2127361c.png)

1-3.選擇對應的GUI版本

![image](https://user-images.githubusercontent.com/103306835/167972992-370792de-f0c7-4cdd-ac17-d7da570a00ef.png)


1-4.下載後解壓縮

1-5.開啟sqlectron

![image](https://user-images.githubusercontent.com/103306835/167973456-485b1160-8c1f-49a7-96b2-e061cd966c9c.png)


2.sql檔：https://github.com/EISCFCU/BI_SAS/blob/main/insertposdata.sql


# 操作步驟

![image](https://user-images.githubusercontent.com/103306835/169325833-78f2025b-5939-41f5-aaf5-4055e56104a4.png)

# Step1：建立雲端資料庫

1.點選[RDS]

![image](https://user-images.githubusercontent.com/103306835/169428952-fc0c25dd-2b61-41d8-a889-1548d1a5e913.png)

2.點擊[創建資料庫]

![image](https://user-images.githubusercontent.com/103306835/169428975-0eb2ed1c-4cae-447c-84c8-8e35135b82ee.png)

3.選擇[標準建立]

![image](https://user-images.githubusercontent.com/103306835/169428999-00870f14-73a7-486d-b7c7-53161fcd3313.png)

4.選擇 PostreSQL

![image](https://user-images.githubusercontent.com/103306835/169429073-6959a751-f114-4929-899e-7c1e063f66e9.png)

5.選擇免費方案

![image](https://user-images.githubusercontent.com/103306835/169429092-6c0cf056-0792-45c6-9b2d-6a617cc9f246.png)

6.資料庫設定

資料庫實例標識符 ：database-3 

主要使用者名稱：postgres 

主要密碼：pass1234 

確認密碼：pass1234

![image](https://user-images.githubusercontent.com/103306835/169429172-8fc83d8c-b798-44cf-b4a4-8e0bc0fe67dc.png)

7.資料庫執行個體類別->選擇爆量類別 (包括 t 類別)

![image](https://user-images.githubusercontent.com/103306835/169429414-02ffba5b-079c-4ad3-9482-851d576877a0.png)

8.Virtual Private Cloud (VPC)：Defalt VPC

![image](https://user-images.githubusercontent.com/103306835/169429459-e33a8317-4562-40bb-baad-adf47148105a.png)

9.公開存取：是

![image](https://user-images.githubusercontent.com/103306835/169429496-245ff79e-c312-4956-9b7d-ae0df495ec44.png)

10.選擇現有的VPC安全群組：default

![image](https://user-images.githubusercontent.com/103306835/169429530-b4f966bc-267b-437a-babb-65a9536879e2.png)

11.展開其他組態

![image](https://user-images.githubusercontent.com/103306835/169429552-8e348101-3392-4f50-a316-24af4fd12de6.png)

12.初始資料庫名稱：lab

![image](https://user-images.githubusercontent.com/103306835/169429721-7e18de14-c9ad-4284-a114-18c3518fe689.png)


13.取消勾選[啟用增強監控]與勾選[啟用刪除保護]

![image](https://user-images.githubusercontent.com/103306835/169429812-4f407e94-40c3-43f4-b9ff-f27b4e71b79c.png)

14.點選[建立資料庫]

![image](https://user-images.githubusercontent.com/103306835/169429841-e5c02a2c-6fb9-426a-afa9-8f7596ddaea1.png)

15.等待建立完成(狀態變成可用)

![image](https://user-images.githubusercontent.com/103306835/169429868-8a88fa56-e1f0-4c11-a67a-9205154e9420.png)

# 步驟2：連線到RDS 

1.確認RDS Security Group 的inbound rule 的來源為0.0.0.0/0

2.開啟sqlectron

![image](https://user-images.githubusercontent.com/103306835/169430427-140ea28f-5744-4e13-9a4d-85784280707d.png)

3.點選[Add]

![image](https://user-images.githubusercontent.com/103306835/169430450-7ee6411a-416f-4c83-9867-5913ef74720d.png)

4.輸入資料庫連線

![image](https://user-images.githubusercontent.com/103306835/169430640-7c135894-6881-400b-8590-170b578b0dc9.png)

5.點選[Save]

![image](https://user-images.githubusercontent.com/103306835/169430665-147620f4-ca0f-4525-afe4-8c5952fad33a.png)

6.點選[Connect]

![image](https://user-images.githubusercontent.com/103306835/169430686-70029b84-c5ea-4d4d-b2a4-626e4e68d5aa.png)

# Step3：匯入資料

1.貼上CREATE Table語法

```
CREATE TABLE IF NOT EXISTS public.pos
(
	city varchar(255), 
	name varchar(255),
        orders_total double,
        s_year varchar(255),
	s_month varchar(255),
	s_day varchar(255),
	s_quarter varchar(255), 
	s_hour varchar(255),
	orders_count int
);

CREATE TABLE IF NOT EXISTS public.area
(
    id varchar(255),
    name varchar(255)
);

CREATE TABLE IF NOT EXISTS public.payment
(
    id varchar(255),
    name varchar(255)
);
```

![image](https://user-images.githubusercontent.com/103306835/169430726-54ae2e89-b9f8-48ba-a6cb-b9b59d81cff1.png)

2.點選[Execute]

![image](https://user-images.githubusercontent.com/103306835/169430787-ddcae7d8-f250-430f-9ef7-f1d8fad09369.png)

3.點選[File]

![image](https://user-images.githubusercontent.com/103306835/169430809-ad982514-f160-4866-8c3c-75ebc60ae21c.png)

4.點選[Open Query]

![image](https://user-images.githubusercontent.com/103306835/169430847-786d1fe2-d9ae-4ed9-9623-636d092dc4f0.png)

5.選擇insertposrds.sql

檔案下載連結：https://github.com/EISCFCU/BI_SAS/blob/main/insertposdata.sql

6.點選[Execute]

![image](https://user-images.githubusercontent.com/103306835/169430889-6a620507-8324-420c-b43d-f3b3ddb526f2.png)

7.點選public.pos 顯示資料表資料(public.payment、public.area資料表亦有資料)

![image](https://user-images.githubusercontent.com/103306835/169430918-948d64c8-e24b-44a9-8b8c-5f4ab8b54aca.png)


# Step4：設定檢視表(ViewTable)

1.貼上新增檢視表語法

```
CREATE  VIEW "public".posdata AS SELECT area.name AS area,    payment.name AS payment,    pos.orders_total,    pos.s_year,    pos.s_month,    pos.s_day,    pos.s_quarter,    pos.s_hour,    pos.orders_count   FROM pos     LEFT JOIN payment ON pos.name::text = payment.id::text     LEFT JOIN area ON area.id::text = pos.city::text;
```

![image](https://user-images.githubusercontent.com/103306835/169431097-cce6aa63-8494-4a47-9bbf-84bd0d89dd96.png)

2.點選[Execute]

![image](https://user-images.githubusercontent.com/103306835/169431270-0873068f-f9d8-4216-92cc-cd73d6eca4a0.png)

3.顯示public.posdata檢視表

![image](https://user-images.githubusercontent.com/103306835/169431299-b1ae0ff0-891c-48f0-98de-be14bd60ca6d.png)


# Step5：登入SAS Studio 

SAS Studio登入連結：https://welcome.oda.sas.com/login

1.輸入帳密

![image](https://user-images.githubusercontent.com/103306835/169431384-887880b7-019d-4d30-8a39-f990dcbb7f8c.png)

2.勾選Accept…..

![image](https://user-images.githubusercontent.com/103306835/169431439-5fecb3b8-fcda-471f-a997-abd7bd886bba.png)

3.點選[Sign In]

![image](https://user-images.githubusercontent.com/103306835/169431483-af56a8ca-1acd-4c3e-be35-d729cb73df6e.png)

4.點選[SAS Studio]

![image](https://user-images.githubusercontent.com/103306835/169431503-e26a4688-085b-4e42-adc8-77fc819ad256.png)

# Step7：從RDS下載到SAS

1.SAS Studio

![image](https://user-images.githubusercontent.com/103306835/169431557-5b0f2e11-3ba6-4450-9da0-4ca65bea4344.png)

2.點選[新增]

![image](https://user-images.githubusercontent.com/103306835/169431577-b2d78909-174f-4455-912e-96a78463795e.png)

3.點選[SAS程式] 開啟程式檔

![image](https://user-images.githubusercontent.com/103306835/169431612-6b156917-2b2d-4fc2-ab08-48fc09c1830d.png)

4.貼上程式碼

```
* Using LIBNAME engine;
libname AWS_RDS postgres
 server="database-3.crxpcyzinmjk.us-east-1.rds.amazonaws.com"
 user="postgres" PW="pass1234" database="lab" schema="public"
 port=5432;

options sastrace=',,,ds' sastraceloc=saslog nostsuffix ls=64;
;
run;
options sastrace=off;

```
![image](https://user-images.githubusercontent.com/103306835/169431655-7c4aefce-00c6-48ac-ab52-739c5f421b7c.png)

5.修改server(Endpoint)

![image](https://user-images.githubusercontent.com/103306835/169431677-f447ff87-6656-4784-b301-784d4664d9b4.png)

6.點選[執行]

![image](https://user-images.githubusercontent.com/103306835/169431696-35aa6676-6b4d-4cfd-91c3-bd1fe9b0e841.png)

7.產生AWS_RDS資料館

![image](https://user-images.githubusercontent.com/103306835/169431707-66312be4-cc08-4311-b561-36fefc958d9d.png)

8.成功匯入資料

![image](https://user-images.githubusercontent.com/103306835/169431747-667b69c4-7a5f-46fc-8b22-896ea0689114.png)

# Step8：SAS資料分析

實作：統計各地區別訂單的人數並以圓餅圖/長條圖呈現

實作：統計各種付款方式的人數，並以長條圖呈現

實作：統計各種付款方式的地區分布，並以圓餅圖呈現

實作：統計不同訂單數量的人數，並以直方圖呈現

實作：以散佈圖檢驗訂單數與付款金額間是否有相關性

實作：以相關分析方法檢定訂單數與付款金額間相關係數

實作：以單因子次數分析查看基本統計資料(次數、百分比、累積次數)

實作：以單因子ANOVA分析，檢定不同城市與其訂單量間是否有相關性存在




