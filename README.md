# 📌 STRICTLY READ BEFORE PROCEEDING

Bali ganyan ang magiging formatting ng project natin. I'm going to expect na kayo narin gagawa ng database nyo so **READ** this carefully and let this serve you as your **GUIDELINE**  

```
SIS/
├── src/
│   ├── main/
│       ├── java/
│       │   └── com/
│       │       └── plm/
│       │           ├── sis/
│       │           │   ├── database
│       │           │   ├── frames 
│       │           │   └── model
│       │           └── main
│       └── resources/
└── pom.xml
```

![image](https://github.com/jiecolao/student-information-system/assets/137901217/3c937ae8-88c6-4ad3-8572-30aee13be59e)

`com.plm.sis.database` - dito mo mahahanap yung class file for interaction between our *source code* and the *database*. <br>
`com.plm.sis.frames` - dito niyo lagay frames niyo (*naturuan ko naman kayo pano gumawa frames sa netbeans*). <br>
`com.plm.sis.model` - andito yung class file na paggagamitan niyo as reference sa current user. <br>
`Test Packages` - if may gusto kayong itrial and error, dito niyo gawin. <br>
`Other sources > resources` - dito niyo upload yung mga gagamitin na necessary jpegs. **INDICATE NIYO FILEPATH NETO IF EVER MAN NA MAGUUPLOAD KAYO DITO LIKE UNG PROFILE PIC, PDF, ETC.** <br>
`pom.xml` - Kapag may bago kayong jars na nilagay, update nyo to.
<br>

> [!NOTE]
> Kapag nalink nyo na, check niyo mga class files sa bawat packages, may mga comments jan na naka-elaborate na.

<br><br>

## 🔷 SETTING UP THE PROJECT SA NETBEANS NYO

> [!NOTE]
> Hindi mo idodownload to ha, iclone mo para makapush and pull ka.

Clone[^1] this project via git using the github link of this project
### 🔗 https://github.com/jiecolao/student-information-system.git
<br> 
After niyo malink,

<br> <br>

## 🔷 AS FOR THE DATABASE TABLE LAYOUT

> [!NOTE]
> May susundan tayong basis for naming columns.

> Student ID = `stud_id` <br>
password = `stud_pass` <br>
name = `stud_name` <br> <br>
... and so on, you get the idea na.

Make sure na kung ano yung column name, ayun rin ang ilalagay niyo sa sql commands niyo <br>
Ganun narin sa table names. <br>

Naka automatic naman na mag crecreate mga to. <br> 
Itake note niyo lang yung names ng **TABLE** and **COLUMN** pati yung corresponding **DATA TYPES** nila

* *`users` TABLE*

| **stud_id** | **stud_pass** |
| --- | --- |
| 202212345 | 123qwe |
| *null* | *null* |

* *`info` TABLE*

| **stud_id** | **stud_name** | **stud_email** | **stud_contact** | **stud_col** | **stud_crs** | **stud_type** | **stud_yrlvl** |  
| --- | --- | --- | --- | --- | --- | --- | --- |
| 202212345 | Jograt | myemail@gmail.com | 09151234567 | CISTM | CS | regular | 1 |
| *null* | *null* | *null* | *null* | *null* | *null* | *null* | *null* |

* *`grades` TABLE* how sa pdf tho

| **stud_id** | **grd_yr** | **grd_sem** | **grd_subj** | **grades** |
| --- | --- | --- | --- | --- |
| 202212345 | 1 | 1 | CSC | 1.00 |
| 202212345 | 1 | 2 | DSA | 1.25 |
| *null* | *null* | *null* | *null* | *null* |

> [!IMPORTANT]
> NAKA FOREIGN-KEY DAPAT SA `users` TABLE YUNG IBANG TABLES.

<br> <br>

## VVV YT TUTORIALS ARE LINKED AT THE FOOTER VVV
[^1]: How to link github to Netbeans projects 🔗 https://youtu.be/UOIPS-ewFHg?si=D6DL5SrgkqCaMw_O
[^2]: To add line breaks within a footnote, prefix new lines with 2 spaces.
  This is a second line.
