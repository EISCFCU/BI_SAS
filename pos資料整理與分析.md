


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

```
INSERT INTO "public"."area" ("id", "name") VALUES ("1", "台中");
INSERT INTO "public"."area" ("id", "name") VALUES ("2", "嘉義");
INSERT INTO "public"."area" ("id", "name") VALUES ("3", "新竹");
INSERT INTO "public"."area" ("id", "name") VALUES ("4", "南投");
INSERT INTO "public"."area" ("id", "name") VALUES ("5", "雲林");
INSERT INTO "public"."area" ("id", "name") VALUES ("6", "彰化");
INSERT INTO "public"."area" ("id", "name") VALUES ("7", "苗栗");
INSERT INTO "public"."area" ("id", "name") VALUES ("8", "桃園");
INSERT INTO "public"."area" ("id", "name") VALUES ("9", "金門");
INSERT INTO "public"."payment" ("id", "name") VALUES ("1","cash");
INSERT INTO "public"."payment" ("id", "name") VALUES ("2","linepay");
INSERT INTO "public"."payment" ("id", "name") VALUES ("3","creditcard");
INSERT INTO "public"."payment" ("id", "name") VALUES ("4","Ubereat");
INSERT INTO "public"."payment" ("id", "name") VALUES ("5","foodpanda");
INSERT INTO "public"."payment" ("id", "name") VALUES ("6","easycare");
```

```
CREATE  VIEW "public".posdata AS SELECT area.name AS area,    payment.name AS payment,    pos.orders_total,    pos.s_year,    pos.s_month,    pos.s_day,    pos.s_quarter,    pos.s_hour,    pos.orders_count   FROM pos     LEFT JOIN payment ON pos.name::text = payment.id::text     LEFT JOIN area ON area.id::text = pos.city::text;
```


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
