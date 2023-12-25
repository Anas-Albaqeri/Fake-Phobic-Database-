Fake-Phobic News
CSC375_project

Dr. Hussein Bakri
Anas Albaqeri
Mohammad Shahin
Yazid Boufous
Table of Content:
1- Introduction:
2- Tools used to draw the ER
3- System Description & Requirements:
4- Legend of ER diagram symbols:
5.1 Full ER Diagram
New ER: (PHASE 2)
5.2 Entity Types & Their Attributes
Employee:
Publication:
Article:
News Portal:
Subscription Plan:
Advertisements:
Supplier, Items & Inventory:
Distributor:
5.3 Relationships and Their Explanations
The changes done for phase2:
6- ER to Relational Mapping:
6.1 Step 1 – Mapping Strong Entity Types
6.2 Step 2 – Mapping of Weak Entity Types
6.3 Step 3 – Mapping of Binary 1: 1 Relationship Types
6.4 Step 4 – Mapping of Binary 1 : N Relationship Types
6.5 Step 5 – Mapping of Binary M : N Relationship Types
6.6 Step 6 – Mapping of Multivalued attributes
6.7 Step 7 – Mapping of N-ary
7- Full Display: (Phase 2)
8- Table State:
9- Table Structures (SQL):
10.DATA INSERTION:
11- Queries Executed:
12- Normalization:
13- Conclusion:
14- References:
1- Introduction:
Newspapers were oncethe strongest tool for communicating informationto people.
Although technologicaladvancements havesignificantlyreducedtheusage ofspecificallyin

theirphysicalform, theyarestillconsideredone themostimportantmedia platformstoday.

Newspapersarereliablesourcesthatensurevalidationanddeepinvestigationofinformationand

events,grantingthemanadvantagethatmightbemissingfromothermediaplatforms.Easeof

accessandwideavailabilityareotheradvantagesthatnewspapersprovideoverothersources.

Moreover,newspapersarepublishedin multiplelanguages,makingthem moreaccessibleto

people from different regions. However, therearemanykeyelementsthatmake upa good

newspaper today, ranging from online availability to good distribution services.

Fake-PhobicNewsisthenewbignewspaperintown.Ourgoalistodelivercrediblenews
thatthereadersdeservetoread.Wecarealotaboutourreadersandso,hereatFake-Phobic

News,wefocusalotonouronlinenewsportalservicesinorderforournewstobereachableto

thebiggestnumberofusersglobally. Ourreaderscaneasilysign-upforouronlineservices,

create their personal accounts, and choose the best suitable subscription for them.

Diversityandinclusivityareothertwofactorsthatmakeournewspaperthefirstthingpeople

wanttoreadinthemorning,asFake-Phobicmakessuretohavenewsfromdifferentgenresand

placesforeveryreaderoutthere.Fake-Phobicensureshavingmultipleauthorsandjournalists

that cover various numbers of topics that give every reader a bit of their tastes and interests.

Anycompanyneedsgoodmanagementtosucceedandtherefore,weatFake-Phobicgive
afairshareofattentiontoouradministrationofthecompany.Ensuringtheflowofworkthrough

adequatemanagementofoursuppliesofpapersanddifferentofficeutilitiesisoneoftheprimary

tasks that our administration excels at.Additionally, ouradministrationmakessure thatour

printed papers are properly delivered and distributed to our loyal customers.

AsFake-PhobicNewsisbecomingthetalkofthestreetsrapidlyduetoitsamazingservices,we

haveaccountedcarefullyforprovidingthebestplatformforadvertisements.HereatFake-Phobic

News, clientscaneasilychoose thebestplanfromourmultipleflexibleoptionsthatfittheir

needs in advertising.

As Fake-Phobic News is growing rapidly to become the pioneer of thenewspaper
industry,ourresponsibilitiesand managementaregetting wider.Weenvisionafuturewhere

newspapersareasrelevantastheyusedtobewhenfirstintroducedtotheworld.Therefore,our

team dedicatestheir completeskills andknowledgein managementand technicalsupportto

deliverwhatthepeoplewanttoread.YazidBoufous,ourdirectorofediting,makessurethatour

readers havememorable and interestingtopics to discuss with their friends andcolleagues

throughout the day after reading our newspaper as their morning routine. In parallel, our

advertisementsadministrator:AnasAlbaqeirmakessurethatclientsarefindingthebestoffersto

placetheirdifferentadvertisementsandannouncements.Ontheotherhand,ourgeneralmanager

MohammedShahin makessureofthecontinuousflowof operationsatthecompanyandits

differentdepartmentsfromadministrationtoauthorsandeditors,andeventuallydistributionand

delivery.

AtFake-PhobicNews,ourteamworkstirelesslytoensurethatourreadersdevourcrediblenews,

enjoy what they read, and learn something new every time they open our paper or website.

______________________________________________________________________________
______________________________________________________________________________
2- Tools used to draw the ER
The tool that our team has used to implement the ER Diagram isdraw.io. This tool has
provided us with a collaborative environment to work on one collective vision. The fluidity and
simplicity of the platform have made it convenient for us to connect and implement our ideas,
since there is a wide variety of diagrams offered for all use.

3- System Description & Requirements:
Our system consists of 12 main entities with each of them having attributes.More
information will be provided about each entity, attribute, and relationship in section 1.

● EachpublicationisidentifiedbyanISSNandhasaheadline,adateofpublication(Day,
month,year),anumberofcopies,issue,volume,atypeofpublication,andanumberof
pages.

● Eachpublicationiscomposedofarticles.EveryarticleisidentifiedbyanarticleID,and
hasatitle,byline,author,body,photo,keywords,andadatelinecomposedofadateanda
location.

● Everypublicationcontainsadvertisements.EachadvertisementhasakeyofanAD_ID,a
size, a position, price, template.

● Any advertisement must be owned and requested bya client.Thelatteris uniquely
identified through a Client_ID. We record the name, the email, the phone and the address.

● Oursystemalsocontainsanonlinenewsportalwhereourpublicationswillbepublished
sothatouronlineuserscanhaveaccesstothem.Theportalhasauniquedomainanda
regionwhereitisavailable.Theportalauthenticatesusersthatcanaccessthedifferent
publications.Everyuserisassignedauniqueuseridandusername,andhasajoining
date, contact info made of name, email, and address.

● Every userissubscribed toa subscriptionplanthathasa subscriptionnumber,type,
period, status, and a price.

● EmployeesinthenewspaperhaveauniqueID,aname,age,email,phone,salary,sex,an
addresswith thecountry,city,street, andzipcode.Wealsostore thepositionofthe
employee.

● Anemployeecanbeasupervisorofanotherone,andhasdependantsthathaveaname,
sex, age and relationship to the employee.

● An employee caneither havean administrativeor a non-administrativeposition. A
non-administratorworksforadepartmentandonanarticlefromwherewecanrecordthe
workinghours,butcanalsomanageadepartmentfromwherewecanrecordthestarting
date. The employee can also communicate and coordinate with the suppliers.

● A department is uniquely identified by its name and a number.

● OursuppliersareuniquelyidentifiedthroughasupplyID.Everysupplierhasanameand
an address.
● A suppliersupplies items. Each of thelatter has a unique barcode, aname anda
category.
● Distributorsareneededtopublishourhardcopycopies.DistributorshaveanID,aname,
andaddressandregionofdistribution.Thequantityandthefrequencyofthedistribution
should also be stored.

4- Legend of ER diagram symbols:
______________________________________________________________________________
5.1 Full ER Diagram
OLD ER:
New ER: (PHASE 2)
NEW ER: PHASE(3)

5.2 Entity Types & Their Attributes
Employee:
Employeesarethebeatingheartofanycompany.Ournewspaperkeepsadetaileddescriptionof
each employee at the company.
Our Employee entity has the following attributes:
● ID : The key attribute of an employee, as every employeehas a unique ID
● Name : A composite attribute that holds the first andlast names of our employees
● Sex : an attribute to store employees' sex: whethermale, female or other.
● Email :Everyemployeein thecompanyhasa uniquecompanyemailastheprimary
professional communication tool.
● Address :acompositeattributethatcomprisesthefoursub-attributes:country,city,zip
code, and street, all put together, giving us a clear record of where employees live
● Salary: an attribute that holds the wage informationof each employee.
● Phone: a multivalued attribute that holds the phonenumber/s of each employee.
● Age: a derived attribute that tells how old each ofour employees

Publication:
The publication entity is the umbrella under which falls every published work of our newspaper
including articles, advertisements, online posts.. etc.
The following are the attributes of the publication entity:
● Volume: is an attribute that represents the exactvolume (group of issues) of the
newspaper <i.e. Fake-Phobic News , 6 - 21>
● ISSN: is the key attribute that represents the standard8-digits serial number that
uniquely identifies the publication.
● Issue: is the basic number of the exact single newspaperpublication that belongs to a
group of the issues (a volume) i.e.: <Fake-Phobic News , 6 - 21 >
● Date of publication: is a composite attribute thatholds the date when the publication
(the exact issue of the newspaper) was made, including the day, month and year. i.e.:
<Fake-Phobic News , 6 - 21, December 12, 2022>.
● Publication type: is the attribute that indicateswhether we have a printed publication or
an online one.
● Language: is an attribute that holds the languageused for a single issue / publication. i.e:
<Fake-Phobic News , 6 - 21, December 12, 2022, ENG >.
● No. of pages: is the attribute holding the numberof pages in the publication.
● No. of Copies : is the attribute representing thenumber of copies of each publication
made.

● Headline: is the attribute holding the title or headline of the newspaper. i.e
(<Fake-Phobic News , 6 - 21, December 12, 2022, ENG - “A Girl on Tik-Tok Sells one
of Her Kidneys for Views” >
Article:
Ifemployeesrepresenttheheartofthecompany,thenthearticlesofournewspapersrepresent
thebloodofthenewspaper.Anewspaperisessentiallyagroupofarticlesandsothisisoneof
the main entities that has the following attributes:
● Article ID: a key attribute that holds each article’sunique ID number.
● Title: an attribute that holds each article’s title.
● Body: an attribute that holds each article’s bodyparagraphs.
● Keywords: amultivaluedattributethatholdsthemainterminologiesandconceptsused
in each article.
● Photo: an attribute that holds photos that are usedin the articles.
● Byline: an attribute that holds the name of the article’sauthor.
● Dateline: acompositeattributethatholdsthedateandplaceofwhen(Date)andwhere
(Location) the article was written.

User:
As a newspaper, our biggest stakeholders are customers and so our users for theonline
newspaper portal is a major entity that have the following attributes:
● User_ID: isakeyattributeholdingtheusers’uniqueIDsoftheonlinenewspaperportal
(page).
● Username: is another key attribute holding the usernameof the page user.
● Password: is an attribute that holds each page user’spassword.
● Date joined: is an attribute that holds the user’ssubscription date.
● ContactInfo: is yetanothercompositeattributethatholdsthecontactinformationof
each page user. It consists of the( Name, Email, andAddress).

Client:
A client is yet another important entity that represents advertisement clients; one of the most
important stakeholders in our company.
The client entity has the following attributes:
● Client ID: is the key attribute that holds the clients'ID for our newspaper (i.e
Xcompany#)
● Email: is the multivalued attribute that holds theemail/s of our advertising clients.
● Address: is a composite attribute that holds the addressof the client (country, zip_code,
street, city)

● Phone: is another multivalued attribute that holds the phone number/s of our clients.
● Name: is a composite attribute that holds the firstand last names of our clients.

Department:
The Department is an entity that identifies the different categories we have in the newspaper such
as sports, politics, kitchen.....etc
The two following attributes are defined for the Department entity:
● Number: is a key attribute of the Department entityholding the company-assigned
number of each category of the newspaper.
● Name: is another key attribute of the Department entitythat holds the name of each
category or department in the newspaper i.e (Sports, Politics...etc.)
● Phone : is a multivalued attribute that holds all thephones and extensions of the
department
● Email : is a multivalued attribute that contains theemails of the department

News Portal:
The newsportalisa veryimportantentity thatrepresentstheonlinepartofourcompany’s
services.Anewsportalisasubscription-basedwebsitethatpublishesanelectronicversionof
our printed newspaper.

The news portal has the following two attributes:
● Domain: is the key attribute that holds the domain(URL) of our online page.
● Region: is anattributethat determinesthat holdstheexactregionthenewsportalis
covering.

______________________________
Subscription Plan:
The subscription plan is a vital entity that provides users various options for our services at their
convenience.
The subscription plan has the following attributes:
● Type: is an attribute that holds the type of subscriptionthe user has (i.e; premium,
standard... etc.)
● Period: is the attribute that holds data regardingthe duration of subscription the user has.
● Price: is an attribute holding the price of each subscription.
● Subscription Number : is the key attribute that holdsa unique number of the user
subscription

Advertisements:
Theadvertisemententity isanotherimportantpartofournewspaper.Itrepresentsoneofour
primary sources of income for the company.
The following are the attributes of the advertisement entity:
● AD_ID: is the key attribute that holds each advertisement'sunique ID.
● Size: is the attribute that holds the size of eachadvertised ad in our newspaper.
● Page: is the place the attribute that holds the number of the exact page that the
advertisement on.
● Template: isanattributethatholdsthedifferentmoldsandformsofadvertisementsthat
weprovidehereinFake-PhobicNews.Templatesofadvertisementsdisplaythesizeand
position.
● Price: isan attributethatholdstheinformationonthecostofeachadvertisementitwill
be depending on the size, position and page of the advertisement.

______________________________________________________________________________

Supplier, Items & Inventory:
Thesetwoentitiesarestronglycorrelatedandsowe
discussthemasapair. Supplier entityrepresentssupplyingcompaniesthatournewspaperneeds
forpapersandofficeutilities,while Items entityrepresentstheitemssuppliedfromthesupplier
to the publication that will use them later when creating physical copy.
The following are the unique attributes for the entities:
a. Supplier:
● SupplyNo. isthekeyattributerepresentingtheuniquenumberofeachsupply
shipment for the company.
● Address: isa compositeattribute containinga(country,zip_code,street,city)
representing the location of each supplier company.
● Name: isa compositeattributerepresentingthenameofthesuppliercompany
(i.e. Trexy Paper.Co )
b. Items :
● Barcode: is thekey attribute that holds the uniqueID.
● Category: is the classification of item stored
● Name: is a simple attribute of the name of the item

_________________________________________________________________
Distributor:
Distributorisa weakentity thatexists dependingontheprintedpublication'sexistence.The

following are the attributes associated:
● Name: is the attribute holding the name of the distributingcompany.
● DistributorID: isnotakeybuttheattributethatalongwithpublicationtypeandID
(foreign key) make up the primary key for the entity.
● Address: is an attribute holding the location of eachthe distribution company
● Region Covered: is an attribute that represents theregions each distributor covers.

_____________________________________________________________
5.3 Relationships and Their Explanations
The relationship “Contains” represents the publication containing articles. There exists a
one-to-manyrelationshipbecauseapublicationcancontainmultiplearticles,butanarticlecan
onlybeusedandcontainedinonepublication.Regardingparticipation,itistotalparticipation
for the publication since it can not be published without it containing an article.

Therelationship‘Displays”representsthepublicationdisplayingadvertisements.Itisshownby
many-to-many relationships because a publication can displaymanyadvertisements,and an
advertisementcanbedisplayedinmultiplepublications.Inaddition,anadvertisementcannotbe
displayedunlessapublicationexiststhatexplainsthetotalparticipationoftheadvertisement.
Therelationshipcontainstheattribute“Duration”whichreportsthedurationoftheadandhow
long it will last, meaning whether it will be in every copy for a week, or a month...

Therelationship“Ownedby” showsthatan advertisementmustbeownedorrequestedbya
client for it to be displayed in a publication, which is why ithas total participation.An
advertisement can be only owned by one client. However, a client can request many
advertisements to be promoted, which is why the relationship is many to 1.

Therelationship“Postedon”showsthatthepublicationsarepostedonthenewsportalforusers
to access.Apublicationcanbeonlypostedinonenewsportal.However,thelattercanhave
manypublicationspostedinit,meaningitismanytoone.Itispartialparticipationbecausenot
allpublicationsmustbepostedontheportalsincesomehardcopiesarelimited,thesameway
the portal does not need to have all publications on it.

Therelationship“Authenticate”representstheonlineportalhostinguserssothattheycanhave
accesstothepublications.There existsa1-to-manyrelationshipsincetheportalhosts'many
users; however, the user can be hosted by only one newspaper portal. Theuser has total
participation since they must host all users via a portal.

Therelationship“Follows”displays thatallusersneedtofollowonlyonesubscriptionplan.
Eachplandiffersfromtheothers,sinceeachhasitsownpriceandfeatures.Thatiswhyitwas
representedusingamany-to-oneandtotalparticipationofusers.However,asubscriptionplan
canbefollowedbymanyusers.WerecordtheattributeStartdatefromtherelationtokeeping
track of when the user first enrolled in the subscription.

Three entitiesarelinkedbytherelationship"Supplies": supplier,publication,and item. The
relationship representsthe provision of inventory itemsbya supplierbyprovidingmaterial
mainlylikepaper,ink,printers.Thesameentitycanprovidemanyitems,andasuppliercangive
severalitemsatthesametime.Furthermore,morethanonepublicationcanreceivefromthe
supplier.Thisrelationshiphasattributesfromit:“Cost”,“Quantity” andacompositeof“Dateof
supply” (Day, Month, Year) storing the details needed about the transaction. Also, the
relationship has a cardinality of Many to Many to Many (M:N:P).

The relation “Coordinates with” is a relationship between two entities: a supplier, an
administratoremployee.Theemployee’sroleisto coordinatewiththesuppliers. Butnotall
administratorshavethatroleexplainingthereasonitispartialparticipation.Yet,eachsupplier
mustcoordinatewithanemployee.Furthermore,therelationhasanattribute“Start_Date”that
holdsthedateofcooperationbetweentheemployeeandthesupplier.Finallytherelationhasa
cardinality of Many to Many.

“Supervisor”isarecursiverelationshowingthatanemployeecanbeasupervisorofanotherone.
Anemployeeplayingtheroleofasupervisorcanhavemanysupervisees,butasuperviseecan
only have one supervisor managing him.

The relationship “Produces” represents a department producing an article. It is 1-to-many
relationshipbecauseadepartmentcanproduceseveralarticlesandanarticlecanonlybedirected
by one department. We also say that there cannot bean articlethatis notproducedbya
department.

The“Worksfor”relationshipshowsthatanemployeehastoworkforonlyonedepartment,and
the lattercan have manyemployees butneeds to haveatleast one.This explainsthetotal
participation of both entities in the relationship and the many-to-one choice.

The“Manages”relationshipdisplaysthatanemployeecanmanageonlyonedepartment,butnot
every one of themcandothat role.Thatiswhyitisa partialparticipation.Regarding the
department,onlyoneemployermustmanageitandthatexplainsthepartialparticipationandthe
one-to-onerelationship.Ithasanattribute‘Startingdate”thatwillhelpstorethestartingdateof
the employer’s role as a manager for the department.

The“Workson”relationshipdisplaysthateveryemployeeworksonatleastonearticle,andan
articlemusthaveatleastmanyemployeesworkingonit.Italsohasthe“Workinghour”attribute
thatkeepstrackoftheemployers’workhours.Thatfunctionwill behelpfulwhenexpandingthe
functions of the DB to side better salaries and vacations.

The“Dependantof”isanidentifyingrelationshipthatshowsthedependenceoftheweakentity
dependentonthestringentityemployee,demonstratingthatadefendantcannotexistwithoutan
employee since they do not have a unique id to distinguish them.

The“Distribute”isthesecondidentifyingrelationshipthatdemonstratesthatadistributorisa
weak entity thatdependson thepublicationitself.Meaningwewillnot getthedataofthe
distributor until there is publication to be published. A distributor can distribute many
publications.Thisrelationhas anattributewhich is“Frequency”thatdisplayshowoftenthe
distribution is done along with the quantity distributed. Also the relationhas an attribute
“Quantity Distributed” that holds the amount of copies sold.

The End of Phase 1#
Webeganourinvestigationinthissectionbyidentifyingtheentitiesandrelationsthatrepresent
thefundamentalsneededtosustainanewspaper.Wewillusethissectionasastartingpointfor
thenextpartofourjourney,wherewewillimplementthepreviouslymentionedillustrationsand
conceptsonareal-worldbasistodemonstratetheirvalue.Inordertofacilitatethedigitalization
of the previously mentioned entities and relationsinto actual DBMSmappingsratherthan
limiting theprojecttoanERmodel,academicallylearned,wewillimplementconceptsinthe
following sections:

The changes done for phase2:
Aspartof ourpreparationformapping theER, wereviewedtheresultsthoroughlywiththe
assistanceofourinstructor.Byfollowingtheinstructor'sadvice,wewereabletoimproveour
previous ER. We made the following changes as a result:

● Weremovedboth“Administrator”and“Non-Administrator”entitiesastheywerespurious
entities and replaced them with a binary attribute on the “Employee” entity.
● Consequently, we removedthe “is-a” relationshipbetweenthe previously mentioned
entitiesandwerelinedthepreviousrelationshipsthatwereconnectedtothespurious
entities to the “Employee” entity directly.
● Weremovedtheinventoryentityasitwasambiguousandreplaceditwitha“Storage”
entity that refers to the company's storage units and warehouses.
● Consequently,weremovedtheternary“provide”relationthatexistedbetween“Storage,
Item andpublication” and replacedthe wholegroupcycle withamoredirectsingle
ternary relation called “supplies” which linked the “supplier,Item and publication” entities.
● We changedthe priceattributefrombeingderived toa normalattributesinceitisa
stored attribute by nature.
● Similarly,wealso changedthe “Template”derived attributefromthe“Advertisement”
entity to a normal attribute.
● We also deleted the “Features” derived attribute in the “Subscription-plan” entity.
● We edited the “Coordinate” relation from a ternary relation linking “Administrator,
DistributorandSupplier”toabinaryrelationcalled“Coordinateswith”thatlinksbetween
employee and supplier in a (M:N) many to many cardinality.
● Likewise, weremovedthe derived“Language”attributefromthe“Newsportal”entity.
SinceitdoesnotcorrelateitwiththeDBMSoftheNewspaper,butratheranapplication
level option of the Newspaper.
● Moreover,wenoticedthatthe“Department”entitylackeddetail,thuswedecidedtoadd
more attributes.
● Additionally,inthe“Article”entity,wenoticedthatthe“keyword”attributeneededtobe
multivalued and so we changed it accordingly.
● Furthermore,werenamedthebinary“Hosts”relationshipto“Authenticate”toprovidea
betterunderstandingoftheconcept,sincetheportaldoesnothosttheusersbutitgives
them access.
● Additionally, we renamed the “Distributes” relationship to “Distribute”.
______________________________________________________________________
6- ER to Relational Mapping:
6.1 Step 1 – Mapping Strong Entity Types
Every strong entity will be transformed into a table known as a relationship table in this step. All
attributes will be included in this table (Except for multivalued ones). We will list the simple
attributes of composite attributes as well.
We have the following Strong entities: Employee ,Article, Department, Client, User,
Publication, Advertisement , News Portal, Subscription Plan , Items and Supplier

1- Employee:

The employee entity contains a mix of many types ofattributes including one multivalued
attribute phone that is not included in the table,a derived attribute Age also not included in the
table, two composite attributes: Address and Name that are represented by their simple
attributes. The rest are simple attributes including the primary key underlined E_ID.

2- Article:

The Article entityincludesonemultivaluedattribute( keywords) whichisnotincludedinthe
table.Additionally,theentityhasonecompositeattribute( Dateline) whichisrepresentedbyits
simple attributes of Date and Location. The rest of the attributes are all simple attributes.

3- Department:

The Department entityhasaKey“Dep_num”,whichisauniquenumberforeachdepartment.
Additionally,wehaveanothercandidatekeyDep_nameandtherelationship Manages attribute
Mgr_start_date.

4- Client:

The Client entityincludesthecompositeattributes name and address thatarerepresentedby
itssimpleattributes.Moreover,theclientincludestwomultivaluedattributes( phone,email )that
are not represented in the table.

5- User

The User entity has a composite attribute of contactinfo represented by its simple
attributes( Name,email,address ). Moreover, the relationincludes the attribute
Subscitpiton_start_date of the relationship Follows.The reset of the attributes are simple
including the primary key underlined User_ID.

6-Publication:

The publication entity has a primary key ISSN whichis the International Standard Serial
Number , and other simple attributes.

7- Advertisement:

The Advertisement entity has a primary key AD_ID andother simple attributes.

8- News Portal:

The News Portal entity includes only two simple attributesincluding region and the primary key
underlined Domain.

9- Subscription Plan

Subscription plan entity has only simple attributeslisted above including the primary key
underlined subsciption_num

10- Items

Items entity also has only simple attributes includingthe primary key underlined Bar_code.

11- Supplier

Supplier entity has composite attribute Address representedin its simple attributes in addition

to the simple attribute Name, and the primary key Supply No.

6.2 Step 2 – Mapping of Weak Entity Types
This step is very similar to step 1 but instead of having a primary key here , each week entity has
a partial key (pink) that along with the primary key form the parent entity (blue) form the
primary key for the relation.

1- Distributor

The weak entity Distributor has two partial keys Distributor_ID and Distributor_Name. The
partial keys along with the primary key of the parent entity ISSN form the primary key for this
entity. Additionally, it includes the (Distribute) relationship attributes Frequency and
Quantity_D, andincludesother simple attributes.

2- Dependent

The weak entity Dependent has the simple attributesincluding the partial key Depend_Name
that along with the parent entity (Employee) primary key ID form the primary key for the entity.
Others are simple attributes for the weak entity dependant.

6.3 Step 3 – Mapping of Binary 1: 1 Relationship Types
In This step we show the mapping of the only one to one relationship we have and we specify
which foreign key was included to which relation.

1- Manages

This relationship shows that one Employee managesone Department which yields in the
foreing key Mgr_ssn in the Department relation.

6.4 Step 4 – Mapping of Binary 1 : N Relationship Types
In this step we specify mapping of one to many relationships. We include the foreign keys added
to each table along with the names of every relationship that caused the added foraging key as a
title:

1- Posted on

This relationship shows that one publication postedon (N) News Portals yielding the foreign
key portal_Domain in the publication relation.

2- Supervisor

This relationship shows that one Supervisor can superviseas many supervisees yielding the
foregin key Super_ID in the employee relation.

3- Works for

This relationship shows that one Department has (N) Employees working in it giving the
foregin key Dno in the employee relation.

4- Contains

This relationship shows that one Publication has (N) Articles yielding us the foreign key
P_ISSN to the Article relation.

5- Produces

This relationship shows that one Department can produce(N) Articles yielding the foreign key
Dno in the Article relation.

6- Owned by

This relationship shows that one Client can own (N) Advertisements yielding the foreign key
Clinet_ID on the Advertisement relation.

7- Authenticate

This relationship shows that one Domain can authenticateas many Users and thus yielding the
foreign key Domain in the User table.

8- Follows

This relationship shows that one Subscription Plan has many Users following it and thus giving
us the foreign key Subscription_num in the User relation.

6.5 Step 5 – Mapping of Binary M : N Relationship Types
In this step, we specify the relations for the many to many relationships. In each table, the
primary key of the entities that the binary many to many relationship is connecting are added to
the table as well as each relationship attribute.

1- Works on

The relationship Works on link between the two entities Employee and Article and includes
their primary keys respectively in addition to the relationship attribute W_Hours.

2- Coordinates with

The relationship Coordinates with links between theentities Employee and Supplier and
includes the primary keys of both mentioned entities as shown above in addition to the
relationship attribute Start_date.

3- Displays

The relationship Displays link between the two entities Publication and Advertisement and it
includes their primary keys respectively in addition to its simple attribute Duration.

6.6 Step 6 – Mapping of Multivalued attributes
In this step, we specify the tables for each multivalued attribute in our Database. Each table is
named to clearly indicate to which entity each of the following multivalued attributes belong.

1- Employee Phone

The Employee Phone relation holds the primary key E_ID of the strong entity Employee
and in addition to Phone they form the primary key.

2- Department Phone

The Department Phone relation holds the primary key Dep_num of the strong entity
Department and in addition to Phone they form theprimary key.

3- Department Email

The Department email relation holds the primary key Dep_num of the strong entity
Department and in addition to Email they form theprimary key.

4- Article Keywords

The Article Keywords relation contains the primary key Article_ID of the strong parent
entity Article and along with Email, they form theprimary key.

5- Client Email

The Client Email relation holds the primary key Client_ID of the strong entity Client
and in addition to Email they form the primary key.

6- Client Phone

The Department Phone relation holds the primary key Client_ID of the strong entity
Client and in addition to Phone they form the primarykey.

6.7 Step 7 – Mapping of N-ary
Inthisfinalstep,wespecifythemappingofN-aryrelationshipsconnectingmorethanoneentity.
Werepresentouronlyternaryrelationshipsbelowandshowhowitcontainsasforeingkeys,the

primary keys of each entity it is connecting and, in addition; the relationship attributes
themselves.

1- Supplies

Therelationship Supplies istheonlyternaryrelationshipthatlinksbetweenthethreeentities,
Supplier,item and Publication, anditincludestheirprimarykeys respectively.Inadditionit
includes the simple attributes Quantity , Cost andthe Date of Supply.

7- Full Display: (Phase 2)
Phase 3:

8- Table State:
Publication

9- Table Structures (SQL):
FollowingthecreationoftheERdiagramandrelationalmapping,ORACLEExpresswillbeused
to implement the database in the following section:

Publication
CREATE TABLE Publication
(
ISSN VARCHAR(20) NOT NULL,
PRIMARY KEY(ISSN),
Num_Pages INTEGER NOT NULL,
Copies INTEGER NOT NULL,
Headline VARCHAR(50) NOT NULL ,
Issue INTEGER NOT NULL,
Volume INTEGER NOT NULL,
Lang VARCHAR(10),
P_Date DATE NOT NULL,
Publication_type VARCHAR(10) NOT NULL,
Portal_Domain VARCHAR(50),
FOREIGN KEY (Portal_Domain) REFERENCES News_Portal (Domain)
ON DELETE SET NULL
);

Employee
CREATE TABLE Employee
(
FName VARCHAR (10) NOT NULL,
LName VARCHAR (20) NOT NULL,
E_ID VARCHAR(10) NOT NULL ,
PRIMARY KEY (E_ID),
Email VARCHAR(20),
Sex CHAR(1) CHECK(Sex IN (‘F’, ‘M’)),
Salary INTEGER NOT NULL,
Country VARCHAR(30) NOT NULL,
City VARCHAR(20) NOT NULL,
Street VARCHAR(20) NOT NULL,
Zip_Code INTEGER,
Dno INTEGER DEFAULT 0,
SUPER_ID VARCHAR(10) DEFAULT ‘2021055623’,
FOREIGN KEY (Super_ID) REFERENCES Employee(E_ID)
ON DELETE SET NULL
);
—----------------------------------------------------------------------------------------------------------------------------
BEFORE YOU DO THIS COMMAND, CREATE THE DEPARTMENT TABLE FIRST
—--------------------------------------------------------------------------------------------------------------------------
alter table Employee add constraint ForeignKeyDno FOREIGN KEY(Dno) references
Department(Dep_num) ON DELETE SET NULL

E_Phone
CREATE TABLE E_Phone
(
E_ID VARCHAR(10) NOT NULL,
Phone INTEGER NOT NULL,
PRIMARY KEY (E_ID,Phone),
FOREIGN KEY (E_ID) REFERENCES Employee(E_ID)
ON DELETE SET NULL
);

Department
CREATE TABLE Department
(
Dep_Name VARCHAR(10) NOT NULL UNIQUE ,
Dep_num INTEGER NOT NULL,
PRIMARY KEY (Dep_num),
Mgr_ssn VARCHAR(10) DEFAULT 2021055623,
Mgr_start_date DATE,
FOREIGN KEY (Mgr_ssn) REFERENCES Employee(E_ID)
ON DELETE SET NULL
);

Dep_Phone
CREATE TABLE Dep_Phone
(
Dep_num INTEGER,
Phone INTEGER NOT NULL,
PRIMARY KEY(Dep_num, Phone),
FOREIGN KEY (Dep_num) REFERENCES Department(Dep_num)
ON DELETE SET NULL
);

Dep_Email
CREATE TABLE Dep_Email
(
Dep_num INTEGER,
Email VARCHAR(30) NOT NULL ,
PRIMARY KEY(Dep_num,Email),
FOREIGN KEY (Dep_num) REFERENCES Department(Dep_num)
ON DELETE SET NULL
);

Article
CREATE TABLE Article
(
Article_ID VARCHAR(20) NOT NULL,
PRIMARY KEY (Article_ID),
Title VARCHAR(50) NOT NULL UNIQUE,
Body VARCHAR(1000) NOT NULL UNIQUE,
Byline VARCHAR(70) NOT NULL,
Photo BLOB,
Article_Date DATE NOT NULL,
Location VARCHAR(40) NOT NULL,
P_Issn VARCHAR(20),
Dno INTEGER DEFAULT 0,
FOREIGN KEY (P_Issn) REFERENCES Publication(ISSN)
ON DELETE SET NULL ,
FOREIGN KEY (Dno) REFERENCES Department (Dep_num)
ON DELETE SET NULL
);

Keywords
CREATE TABLE Keywords
(
Article_ID VARCHAR(20),
Keyword VARCHAR(10) NOT NULL,
PRIMARY KEY (Article_ID,Keyword),
FOREIGN KEY (Article_ID) REFERENCES Article (Article_ID)
ON DELETE SET NULL
);

Client
CREATE TABLE Client
(
Client_ID VARCHAR (20) NOT NULL,
PRIMARY KEY (Client_ID),
FName VARCHAR (20) NOT NULL,
LName VARCHAR (20) NOT NULL,
Zip_code INTEGER,
Country VARCHAR (30) NOT NULL,
City VARCHAR (20) NOT NULL,
Street VARCHAR (20) NOT NULL
);

Client_Email
CREATE TABLE Client_Email
(
Client_ID VARCHAR (20) NOT NULL,
Email VARCHAR (30) NOT NULL,
PRIMARY KEY(Client_ID,Email),
FOREIGN KEY (Client_ID) REFERENCES Client(Client_ID)
ON DELETE SET NULL
);

Client_Phone
CREATE TABLE Client_Phone
(
Client_ID VARCHAR (20) NOT NULL,
Phone INTEGER NOT NULL,
PRIMARY KEY (Client_ID,Phone),
FOREIGN KEY (Client_ID) REFERENCES Client(Client_ID)
ON DELETE SET NULL
);

Advertisement
CREATE TABLE Advertisement
(
Ad_ID VARCHAR (20) NOT NULL,
PRIMARY KEY (Ad_ID),
Page INTEGER NOT NULL,
Ad_Size Decimal (10,2) NOT NULL,
Template VARCHAR (20) NOT NULL,
Price Decimal(10,2) NOT NULL,
Client_ID VARCHAR (20) NOT NULL,
FOREIGN KEY (Client_ID) REFERENCES Client(Client_ID)
ON DELETE SET NULL
);

User
CREATE TABLE UserK
(
User_ID INTEGER NOT NULL,
PRIMARY KEY (User_ID),
UserName VARCHAR (25) NOT NULL UNIQUE,
Full_Name VARCHAR (50) NOT NULL,
Email VARCHAR (20) NOT NULL,
Address VARCHAR (50) NOT NULL,
Date_joined DATE NOT NULL,
Domain VARCHAR(50) NOT NULL,
Sub_start DATE NOT NULL,
Sub_num INTEGER NOT NULL,
FOREIGN KEY (Domain) REFERENCES News_Portal(Domain)
ON DELETE SET NULL,
FOREIGN KEY (Sub_num) REFERENCES Subscription_Plan(Sub_num)
ON DELETE SET NULL
);

News_Portal
CREATE TABLE News_Portal
(
Domain VARCHAR (50) NOT NULL,
PRIMARY KEY(Domain),
Region VARCHAR (10) NOT NULL
);

Subscription_Plan
CREATE TABLE Subscription_Plan
(
Sub_num INTEGER NOT NULL,
PRIMARY KEY (Sub_num),
Sub_Type VARCHAR(10) CHECK(Sub_Type IN (‘Premium’, ‘Regular’,‘Economy’)),
Period INTEGER NOT NULL,
Status VARCHAR (20) CHECK(Status IN (‘Active’, ‘Pending’,‘Expired’)),
Price INTEGER NOT NULL
);

Items
CREATE TABLE Items
(
Bar_code VARCHAR (15) NOT NULL,
PRIMARY KEY (Bar_code),
Name VARCHAR (50) NOT NULL,
Category VARCHAR (15) NOT NULL
);

Supplier
CREATE TABLE Supplier
(
Supply_No VARCHAR(10) NOT NULL,
PRIMARY KEY(Supply_No),
Full_Name VARCHAR(40) NOT NULL,
Country VARCHAR(30) NOT NULL,
City VARCHAR(20) NOT NULL,
Street VARCHAR(20) NOT NULL,
Zip_Code INTEGER
);

Works_On
CREATE TABLE Works_On
(
E_ID VARCHAR(10) DEFAULT ‘2021055623’,
Article_ID VARCHAR(20),
PRIMARY KEY(E_ID, Article_ID),
W_Hours INTEGER NOT NULL,
FOREIGN KEY (E_ID) REFERENCES Employee(E_ID)
ON DELETE SET NULL,
FOREIGN KEY (Article_ID) REFERENCES Article(Article_ID)
ON DELETE SET NULL
);

Coordinates_with
CREATE TABLE Coordinates_with
(
Supply_No VARCHAR(10),
Co_ID VARCHAR(20),
PRIMARY KEY(Supply_No,Co_ID),
Start_Date DATE NOT NULL,
FOREIGN KEY (Co_ID) REFERENCES Employee(E_ID)
ON DELETE SET NULL ,
FOREIGN KEY (Supply_No) REFERENCES Supplier(Supply_No)
ON DELETE SET NULL
);

Displays
CREATE TABLE Displays
(
P_ISSN VARCHAR(20),
Ad_ID VARCHAR (20),
Duration INTEGER NOT NULL,
PRIMARY KEY(P_ISSN,Ad_ID),
FOREIGN KEY (P_ISSN) REFERENCES Publication(ISSN)
ON DELETE SET NULL,
FOREIGN KEY (Ad_ID) REFERENCES Advertisement(Ad_ID)
ON DELETE SET NULL

);

Supplies
CREATE TABLE Supplies
(
Supply_No VARCHAR(10),
Bar_Code VARCHAR (15),
P_ISSN VARCHAR(20),
PRIMARY KEY(Supply_No,Bar_Code,P_ISSN),
Quantity INTEGER NOT NULL,
Cost FLOAT NOT NULL,
S_DATE DATE NOT NULL,
FOREIGN KEY (Supply_No) REFERENCES Supplier(Supply_No)
ON DELETE SET NULL ,
FOREIGN KEY (P_ISSN) REFERENCES Publication(ISSN)
ON DELETE SET NULL ,
FOREIGN KEY (Bar_Code) REFERENCES Items(Bar_Code)
ON DELETE SET NULL
);

Distributor
CREATE TABLE Distributor
(
ISSN VARCHAR(20),
Distributor_ID VARCHAR(20) NOT NULL,
Distributor_Name VARCHAR(20) UNIQUE,
ADDRESS VARCHAR(40),
REGION VARCHAR(15),
PRIMARY KEY(ISSN,Distributor_ID),
Frequency INTEGER NOT NULL,
Quantity_ID VARCHAR(20) NOT NULL,
FOREIGN KEY (ISSN) REFERENCES Publication(ISSN)
ON DELETE SET NULL
);

Dependant
CREATE TABLE Dependant
(
D_ID VARCHAR(10),
Depend_Name VARCHAR(30) NOT NULL,
Sex CHAR(1) CHECK(Sex IN (‘F’ , ‘M’)),
Relationship VARCHAR(20) NOT NULL,
Bdate DATE,
PRIMARY KEY(D_ID,Depend_Name),
FOREIGN KEY (D_ID) REFERENCES Employee(E_ID)
ON DELETE SET NULL
);

10.DATA INSERTION:
Now that we have set up our Database tables and identified the constraints on each relation, we
move on to populating our Database accordingly.

EMPLOYEE:

Insert into Employee Values ('Hussein' , 'Bakri' , '2021055623', 'Huseinbakri@yaho.frl', 'M',
6000, 'Lebanon ' , 'Beirut' , 'Hamra' , 28035, 0, NULL);
Insert into Employee Values ('Yazid' , 'Boufous' , '298765123', 'yazidbfs@gmail.com', 'M', 1244,
'Morocco' , 'Casablanca’' , 'Sultan' , 21234, 4, '2021055623');
Insert into Employee Values ('Mohamed' , 'Shahin' , '2345123499', 'Mohamedsha@gmail.com',
'M', 1362, 'Jordan' , 'Amman' , 'Bakra' , 19291, 5,'2021055623');
Insert into Employee Values ('Anas' , 'Albaqeri' , '2345123499', 'anas.albaq@gmail.com', 'M',
2987, 'Yemen' , 'Sana' , Yonis , 34251, 2, '2021055623');
Insert into Employee Values ('David' , 'Smith' , '202105493', 'David.smith@hotmail.fr', 'M', 3000,
'USA' , 'Huston' , 'Dober' , 48025, NULL, '2021055623');
Insert into Employee Values ('Jenifer' , 'Bal' , '3795993231', 'jenni.bal@hotmail.fr', 'F', 2300,
'USA' , 'Arizona' , 'Tucson' , 123445, 3, '2345123499');
Insert into Employee Values ('Jonas' , 'Nail' , '9427100644', 'jonasnail@gmail.com', 'M', 1230,
'USA' , 'OHIO' , 'KENT' , 23441, 7, '202105493');
Insert into Employee Values ('Bella' , 'Mon' , '6543897611', 'belamon121@yahoo.com', 'F', 3341,
'UK' , 'London' , 'Ferement' , 32176, 6, '202105493');
Insert into Employee Values ('Jonas' , 'Nail' , '9427100644', 'jonasnail@gmail.com', 'M', 1230,
'USA' , 'OHIO' , 'KENT' , 23441, 7, '202105493');
Insert into Employee Values ('Anny' , 'Mosh' , '2311009865', 'annymosh3@gmail.com', 'F', 900,
'USA' , 'California' , 'LA' , 87262, 9, '2987651234');
Insert into Employee Values ('Jasmine' , 'Alex' , '3318890811', 'jasminealex@hotmail.com', 'F',
1900, 'Spain' , 'Madrid' , 'GETAFE' , 65746, 8, '3795993231');

Department:

INSERT INTO Department Values ('Admin',0,'2021055623','11-MAY-2019');

INSERT INTO Department Values ('Politics',1,’202105493’,'09-JUL-2018');

INSERT INTO Department Values ('Sport',2,’2345122300’,'13-JUNE-2022');

INSERT INTO Department Values ('History',3,’3795993231’,'03-APRIL-2019');

INSERT INTO Department Values ('Education',4,’2987651234’,'16-OCT-2021');

INSERT INTO Department Values ('Technology',9,’2311009865’,'21-FEB-2020');

INSERT INTO Department Values ('Culture',6,’6543897611’,'19-JAN-2022');

INSERT INTO Department Values ('Art',5,’2345123499’,'23-JAN-2021');

INSERT INTO Department Values ('Music',7,’9427100644’,'11-NOV-2021');

INSERT INTO Department Values ('Film',8,’3318890811’,'04-DEC-2021');

Supplier:

INSERT INTO Supplier Values ('6347','Ford','US','New York','Brooklen.32',10001);

INSERT INTO Supplier Values ('2713','JC. Co' ,'US','Manhattan','Street_43',11001);

INSERT INTO Supplier Values ('1343','Rolling Brother inc','UK','London','Newcastle',11011);

INSERT INTO Supplier Values ('1325','Dundder Mufflin papers','US','Dallas','St.21',01101);

INSERT INTO Supplier Values ('5464','Mo Shahin tools','Jordan','Amman','Bushra',11010);

INSERT INTO Supplier Values ('1234','L.D Billar co.','US' , 'Michigan', 'St.76',11011);

INSERT INTO Supplier Values ('5432', 'Zing co.', 'China','Bejin', 'Xis_64', 01101);

INSERT INTO Supplier Values ('5346', 'Triple N utensils', 'China',' Bejin', 'Sin_42', 10010);

INSERT INTO Supplier Values ('9654', 'China NO 1. Co', 'China', 'Bejin', 'Win_39', 10101);

INSERT INTO Supplier Values ('2365', 'Universal', 'UK', 'Manchester', 'Old_traford', 10010);

INSERT INTO Supplier Values ('5687','Inter_nash_co.','US','Ohio', '39_kent',11101);

Subscription Plan:

INSERT INTO Subscription_PlanValues (23845, 'Premium', 2, 'Active', 30);

INSERT INTO Subscription_PlanValues (13245, 'Regular', 4, 'Pending', 17);

INSERT INTO Subscription_PlanValues (42346, 'Premium', 6, 'Active', 30);

INSERT INTO Subscription_PlanValues (33253, 'Economy', 8, 'Active', 9.99);

INSERT INTO Subscription_PlanValues (16432, 'Premium', 1, 'Active', 30);

INSERT INTO Subscription_PlanValues (28456, 'Economy', 0,' Expired', 9.99);

INSERT INTO Subscription_PlanValues (17568, 'Regular', 6, 'Active', 17);

INSERT INTO Subscription_Plan Values (15257, 'Premium', 5, 'Pending', 30);

INSERT INTO Subscription_Plan Values (19865, 'Regular', 0, 'Expired', 17);

Publication:

Insert into Publication Values ('743007', 5 ,20, 'Hussein Bakri Company becomes a unicorn' , 6 ,
31, 'English', '1-SEP-2022', 'Weekly' , 'Fake-phobic.uk');

Insert into Publication Values ('639575', 3 ,40, 'Iran Dissolves Its Akhlaq Police' , 7 , 12, 'Arabic',
'4-DEC-2022', 'Weekly' , 'Fake-phobic.jo');

Insert into Publication Values ('653590', 12 ,50, 'La France écrira-t-elle l' histoire du Qatar?' , 16
, 20, 'French', '6-OCT-2020', 'Weekly' , 'Fake-phobic.fr');

Insert into Publication Values ('934223', 8 ,20, '法国会在卡塔尔书写历史吗' , 2 , 41, 'Chinese',
'21-JAN-2012', 'Weekly' , 'Fake-phobic.us');

Insert into Publication Values ('086263', 4 ,70, 'Brandon: The First Monkey in F1' , 9 , 87,
'English', '27-JUN-2005', 'Weekly' , 'Fake-phobic.us');

Insert into Publication Values ('477183', 2 ,100,'Alcohol is Now legal in Jeddah!',4 , 26,
'Arabic','29-NOV-2020', 'Weekly' , 'Fake-phobic.lb');

Insert into Publication Values ('239398', 10 ,10, 'Pentagon Issue Code Red After Cyber Attacks'
, 6 , 31, 'English', '17-AUG-2018', 'Weekly' , 'Fake-phobic.us');

UserK:

INSERT INTO UserK Values (646457,'Michael.20','Michael','Michael@gmail.com','Ankara',

'11-FEB-2021','Fake-phobic.tu',’11-FEB-2021',23845);

INSERT INTO UserK Values (875675, 'Chris_topher' ,'Christopher', 'Christ@yahoo.com',
'London','4-MAY-2021','Fake-phobic.uk','4-MAY-2021',13245);

INSERT INTO UserK Values (934256, 'Jessica_eng', 'Jessica' ,'Jessica@Lau.edu','Amman',
'12-JUNE-2022','Fake-phobic.jo', '12-JUNE-2022',42346);

INSERT INTO UserK Values (723463, 'Matthew21','Matthew' ,'Matthew_2@Aub.com','Kent',
'6-JULY-/2021', 'Fake-phobic.us', '6-JULY-2021',33253);

INSERT INTO UserK Values (873452, 'Ashley.cooper', 'Ashley', 'Ashley.21@gmail.com',
'Wales','8-SEP-2022', 'Fake-phobic.uk', '8-SEP-2022', 16432);

INSERT INTO UserK Values (235894,'Jennifer_MW', 'Jennifer', 'Jennifer@yahoo.com', 'Irbid'
,'6-SEP-2021','Fake-phobic.jo','6-SEP-2021',28456);

INSERT INTO UserK Values (745268,'Joshua.Sa2','Joshua','Joshua@outlook.com','Boston',
'7-OCT-2022', 'Fake-phobic.us', '7-OCT-2022', 17568);

INSERT INTO UserK Values (046658, 'Amanda_143', 'Amanda', 'Amanda@yahoo' , 'Beirut' ,
'9-NOV-2021', 'Fake-phobic.lb', '9-NOV-2021', 15257);

INSERT INTO UserK Values (435265, 'Daniel.yildrim2', 'Daniel', Daniel@jubilee.com, Izmir,
10/8/2022, Fake-phobic.tu, 10/8/2022, 19865);

Dep_Email:

INSERT INTO Dep_Email Values (0,'Admin@Fake-phobic');

INSERT INTO Dep_Email Values (1,'Politics@Fake-phobic');

INSERT INTO Dep_Email Values (2,'Sports@Fake-phobic');

INSERT INTO Dep_Email Values (3,'History@Fake-phobic');

INSERT INTO Dep_Email Values (4,'Education@Fake-phobic');

INSERT INTO Dep_Email Values (5,'Art@Fake-phobic');

INSERT INTO Dep_Email Values (6,'Culture@Fake-phobic');

INSERT INTO Dep_Email Values (7,'Music@Fake-phobic');

INSERT INTO Dep_Email Values (8,'Film@Fake-phobic');

INSERT INTO Dep_Email Values (9,'Tech@Fake-phobic');

DEP_PHONE:
INSERT INTO Dep_Phone Values (0,123366598);

INSERT INTO Dep_Phone Values (1,173367383);

INSERT INTO Dep_Phone Values (2,183733736);

INSERT INTO Dep_Phone Values (3,103837478);

INSERT INTO Dep_Phone Values (4,134232422);

INSERT INTO Dep_Phone Values (5,135432345);

INSERT INTO Dep_Phone Values (6,125242422);

INSERT INTO Dep_Phone Values (7,162524311);

INSERT INTO Dep_Phone Values (8,366272199);

INSERT INTO Dep_Phone Values (9,126592571);

E_PHONE :
INSERT INTO E_Phone Values('2311009865', 4433177242);

INSERT INTO E_Phone Values('2987651234', 1543143353);

INSERT INTO E_Phone Values('2345123499', 1937368393);

INSERT INTO E_Phone Values('2345122300', 338374489);

INSERT INTO E_Phone Values('202105493', 9165431324);

INSERT INTO E_Phone Values('9427100644', 5299775860);

INSERT INTO E_Phone Values('3795993231', 4482672820);

INSERT INTO E_Phone Values('6543897611', 4474372769);

INSERT INTO E_Phone Values('3318890811', 52918758798);

Client:

insert into Client values ('74359', 'Andrew', 'Daniels', 101001, 'US', 'New York', 'Wall St.');

insert into Client values('74873', 'Mohamed', 'Ali', 110211, 'Qatar', 'Doha', 'Doha St.');

insert into Client values('43215', 'Hary', 'Kane', 110111, 'UK', 'Manchester', 'United St.');

insert into Client values('23415', 'Ali', 'baba', 001011, 'China', 'Beijing', 'Xing Zong St.');

insert into Client values('53423', 'Zinedine', 'Zidane', 110110, 'France', 'Paris', 'Wall St.');

insert into Client values('94351', 'Ahmad', 'Yasin', 101010, 'Palestine', 'Gaza', 'Khan younes St.');

insert into Client values('84321', 'Mohammed', 'Sades', 100001, 'Morocco', 'Rabat', 'Rabat St.');

insert into Client values('72423', 'Naseem', 'Hamed', 110110, 'Yemen', 'Sanaa', 'Altahrir St.');

insert into Client values('65354', 'Aubrey', 'Drake', 111110, 'Canada', 'Toronto', 'JustinB St.');

insert into Client values('52583', 'Reyad', 'Mahrez', 001011, 'Algeria', 'Algeris', 'Wohda St.');

Advertisement:

INSERT INTO Advertisement Values ('371249', 2, 75, 'Vertical', 15000, '74359');

INSERT INTO Advertisement Values ('123478', 5, 144, 'Vertical', 12000, '74873');

INSERT INTO Advertisement Values ('781943', 3, 100, 'Horizontal', 2500,'43215');

INSERT INTO Advertisement Values ('127348',19,70, 'Heading-style',1000,'23415');

INSERT INTO Advertisement Values ('987212', 7, 75, 'Type-7',1500,'53423');

INSERT INTO Advertisement Values ('098123', 3, 90,'Horizontal', '900,94351');

INSERT INTO Advertisement Values ('814375',12, 30, 'Vertical' ,500, '84321');

INSERT INTO Advertisement Values ('871903', 21, 27, 'Type-11' ,750,'72423');

INSERT INTO Advertisement Values ('897891', 1, 100,'Horizontal' , 20000, '65354');

INSERT INTO Advertisement Values ('081239', 19,288, 'Vertical' ,900, '52583');

News_Portal :

INSERT INTO News_Portal Values ('Fake-phobic.tu','Turkey');

INSERT INTO News_Portal Values ('Fake-phobic.lb,'Lebanon');

INSERT INTO News_Portal Values ('Fake-phobic.uk','UK');

INSERT INTO News_Portal Values ('Fake-phobic.jo','Jordan');

INSERT INTO News_Portal Values ('Fake-phobic.us','USA');

INSERT INTO News_Portal Values ('Fake-phobic.fr','France');

INSERT INTO News_Portal Values ('Fake-phobic.es','Spain');

Client_Phone:

INSERT INTO Client_Phone Values('74359', 91629193);

INSERT INTO Client_Phone Values('74873', 30045272);

INSERT INTO Client_Phone Values('43215', 60580808);

INSERT INTO Client_Phone Values('23415', 61556072);

INSERT INTO Client_Phone Values('53423', 61671849);

INSERT INTO Client_Phone Values('94351', 75240354);

INSERT INTO Client_Phone Values('84321', 59429047);

INSERT INTO Client_Phone Values('72423', 80299970);

INSERT INTO Client_Phone Values('65354', 58586267);

INSERT INTO Client_Phone Values('52583', 99090552);

Client_email:

INSERT INTO Client_Email Values ('23415','alix00@gmail.com');

INSERT INTO Client_Email Values ('43215','HaryK77@gmail.com');

INSERT INTO Client_Email Values ('52583','RyadKing@gmail.com');

INSERT INTO Client_Email Values ('53423','zidaneJub@gmail.com');

INSERT INTO Client_Email Values ('65354','Drake01@gmail.com');

INSERT INTO Client_Email Values ('72423','PrinceNaseem@gmail.com');

INSERT INTO Client_Email Values ('74359','Andi12@gmail.com');

INSERT INTO Client_Email Values ('74873','m.ali43@gmail.com');

INSERT INTO Client_Email Values ('84321','MS_dn99@gmail.com');

INSERT INTO Client_Email Values ('94351','AhYasGaz99@gmail.com');

Distributor:

INSERT INTO Distributor Values( '639575', '2332748', 'James
Distribution','London','UK',3,'34241243521');

INSERT INTO Distributor Values( '086263', '1263732', 'LND
Distribution','Paris','France',4,'14531323252');

INSERT INTO Distributor Values( '743007', '1234232', 'Robert Mufflin Co.','NYC','USA',
12,'14324121234');

INSERT INTO Distributor Values( '653590', '1235234',
'RoyaleDistribution','Amman','Jordan', 5,'11324121234');

INSERT INTO Distributor Values( '934223', '1234324', 'DHL Daily', 'Beirut', 'Lebanon',
12, '12341234123');

INSERT INTO Distributor Values( '477183, 3452434', 'Faster Distribution
Co','Ankara','Turkey', 2,'13443112341');

INSERT INTO Distributor Values( '239398', '5463523', 'Osman’s
Distribution','Sanaa','Yemen',3,'23145432511');

Dependant:

INSERT INTO Dependant Values('2311009865','Hussein', 'M', 'Son', '12-JUN-2001' );

INSERT INTO Dependant Values('2987651234','Mona','F','Daughter', '14-FEB-1955' );

INSERT INTO Dependant Values('2345123499','Rima','F','Mom','21-JUN-1099');

INSERT INTO Dependant Values('2345122300','Lamia','F','Sister','17-JUN-2003');

INSERT INTO Dependant Values('202105493','Mohammed','M','Dad', '15-AUG-2005');

INSERT INTO Dependant Values('9427100644','Alie','M','Brother', '23-SEP-2007');

INSERT INTO Dependant Values('3795993231','Alex', 'M','Uncle','28-DEC-1970');

INSERT INTO Dependant Values('6543897611','Niki','F', 'Mom', '09-APR-1992');

INSERT INTO Dependant Values('3318890811','Rihana','F', 'Sister','22-MAY-1994');

INSERT INTO Dependant Values('2311009865','Marshal', 'M','Grandfather',
'21-JUL-1923');

Display:

INSERT INTO Display Values('639575','371249',3);

INSERT INTO Display Values('086263','123478',2);

INSERT INTO Display Values('743007','781943',7);

INSERT INTO Display Values('653590','127348',6);

INSERT INTO Display Values('934223','987212',1);

INSERT INTO Display Values('477183','098123',1);

INSERT INTO Display Values('239398','814375',4);

INSERT INTO Display Values('639575','871903',6);

INSERT INTO Display Values('086263','897891',2);

INSERT INTO Display Values('743007','081239',3);

Supplies:

INSERT INTO Supplies Values( '6347','981239483','639575',200,900,'12-JUNE-2020');

INSERT INTO SuppliesValues('2713','178349713','086263',450,668,'22-MARCH-2021');

INSERT INTO Supplies Values('1343','183482173','743007',230,1288,'8-FEB-2019');

INSERT INTO Supplies Values('1325','985304958','653590',180,243,'13-NOV-2018');

INSERT INTO Supplies Values('5464','283748329','934223',330,120,'24-APRIL-2020');

INSERT INTO Supplies Values('1234','823748329','477183',570,770,'17-JAN-2019');

INSERT INTO Supplies Values('5432','287438937','239398',660,323,'18-AUG-2022');

INSERT INTO Supplies Values('5346','738248273','639575',880,324,'22-JULY-2021');

INSERT INTO Supplies Values('9654','212378432','086263',120,892,'4-MARCH-2020');

INSERT INTO Supplies Values('2365','478529234','743007',90,234,'2-FEB-2017');

Article:
Insert into Article values('943859LB', 'Finally the terror ends in Iran', ' ', 'Mohammed
bobkeer', NULL,'4-DEC-2022', 'Iran','639575', 1);

Insert into Article values('954421US', 'New genetics that can change everything', ' ',
'Mark Twain', NULL, '27-JUN-2005', 'US','086263', 9);

Insert into Article values('239424UK', 'World Cup Updates', ', ', 'Edward Norton', NULL,
'06-OCT-2020', 'France','653590', 2);

Insert into Article values('324958YE', 'China on Fire', '... ', 'Mao Tang' , NULL,
'21-JAN-2012', 'China','934223', 6);

Insert into Article values('893455TU', 'Is the gulf becoming the US branch', '.,. ', 'Nile
Smith', NuLL, '29-NOV-2020', 'Saudi Arabia','477183' ,1);

Insert into Article values('782425QA', 'AI is getting too powerful', ',., ', 'Jack Sparrow',
NuLL, '17-AUG-2018', 'Canada','239398',9);

Works_on:

INSERT INTO Works_On Values('202105493','943859LB',7);

INSERT INTO Works_On Values('2311009865','954421US',8);

INSERT INTO Works_On Values('2345122300','239424UK',7);

INSERT INTO Works_On Values('6543897611','324958YE',12);

INSERT INTO Works_On Values('202105493','893455TU',20);

INSERT INTO Works_On Values('2311009865','782425QA',4);

INSERT INTO Works_On Values('2311009865','430989UA',5);

Coordinates_With :

INSERT INTO Coordinates_With Values('6347','2311009865','11-JUNE-2020');

INSERT INTO Coordinates_With Values('2713','2987651234','12-APRIL-2019');

INSERT INTO Coordinates_With Values('1343','2345123499','11-MAY-2021');

INSERT INTO Coordinates_With Values('1325','2345122300','4-MARCH-2019');

INSERT INTO Coordinates_With Values('5464','202105493','7-JUNE-2020');

INSERT INTO Coordinates_With Values('1234','9427100644','8-AUG-2019');

INSERT INTO Coordinates_With Values('5432','3795993231','4-OCT-2020');

INSERT INTO Coordinates_With Values('5346','6543897611','14-OCT-2022');

INSERT INTO Coordinates_With Values('9654','3318890811','3-AUG-2019');

INSERT INTO Coordinates_With Values('2365','2311009865','7-AUG-2021');

Keywords :

Insert into Keywords values('943859LB', 'Iran_women');

Insert into Keywords values('954421US', 'iq');

Insert into Keywords values('239424UK', 'france');

Insert into Keywords values('324958YE', 'China_fire');

Insert into Keywords values('893455TU', 'gulf, us');

Insert into Keywords values('782425QA', 'Ai, tech');

Insert into Keywords values('430989UA', 'money');

ITEMS :

INSERT INTO Items Values ('981239483','Dunder’s A4','paper');

INSERT INTO Items Values ('178349713','JC pens ','Utensils ');

INSERT INTO Items Values ('183482173','Dundder’s A2','paper');

INSERT INTO Items Values ('985304958','Shahin’s stables','Utensils ');

INSERT INTO Items Values ('283748329','L.D Billar co. chairs ','Chairs ');

INSERT INTO Items Values ('823748329','Zing co. 7d-Colored','Printers');

INSERT INTO Items Values ('287438937','Triple N utensils pins ','Utensils');

INSERT INTO Items Values ('738248273','China NO1. Co PR23','Printers');

INSERT INTO Items Values ('212378432','Universal - LV00','Recording tools');

INSERT INTO Items Values ('478529234','Inter nash co. CD 4500','Recording tools');

11- Queries Executed:
Scenario 1:
OurSupplycoordinatorsinthecompanyhavenoticedthattherehasbeenashortageofsupply
inourcompany,and areworkingto identifytheproblem.ThusastheDBdevelopersinthe
company,wehelp thesupplycoordinatorssolvethisissuebyretrievingthenameandIDof
eachemployeewhosejobistocoordinatewiththesuppliers,and,additionally,thenamesand
ID of their supervisors.

Query:

SELECT FNAME, E_ID
FROM EMPLOYEE
WHERE E_ID IN (SELECT E_ID
FROM EMPLOYEE
WHERE E_ID IN (SELECT CO_ID FROM Coordinates_With) )
//—-------------------------------------------

SELECT FNAME, E_ID
FROM EMPLOYEE
WHERE E_ID IN (SELECT Super_ID
FROM EMPLOYEE
WHERE E_ID IN (SELECT CO_ID FROM Coordinates_With) )

Output:

__________________________________________________________________________

Scenario 2:
AresearchinstitutionisconductingastudyaboutgenderequalityintheMENARegion.They
wanttogatherthemostamountofarticlesandpublicationsaboutthistopic.Theinstitutionhas
reachedouttoustohelpthemwiththisjob.Inordertohelpprovideaidforthisresearch,we
retrievethetitlesofthearticlesofthattopicusingthespecifickeywordsanddatesofpublishing
ordered from the latest to the oldest.

Query:
SELECT *
FROM
(SELECT Article_ID, Title, Article_Date
FROM Article
WHERE Article_ID IN (SELECT Article_ID FROM Keywords WHERE (Keyword = 'france' OR
Keyword = 'Iran_women')))
ORDER BY Article_Date DESC

Output:

__________________________________________________________________________

Scenario 3:

SinceFake-Phobiciscelebratingits10thannualanniversary,wewanttocelebratebyrewarding
ourloyalfans,whicharethe 10 oldestactiveusersontheplatform.Thoseuserswillbegivena
premiumbundle.Weretrievetheoldestusersbytheirsubscriptionstartdateandupdatetheir
subscription to premium accordingly.

Query:
UPDATE Subscription_Plan
SET Sub_Type =
CASE
WHEN Sub_num IN (SELECT Sub_num
FROM (SELECT * FROM Userk
Order By Sub_Start ASC)
WHERE ROWNUM<=3) THEN 'Premium'
ELSE Sub_type
END

Output:

Scenario 4:

Therehavebeencomplaintsabouttheshortageofnewspapersincertainregions.Wewantto
analyzethesituationandfindpropersolutionsbyfirstretrievingthefrequencyofdistributionfor
each region, and the name and IDof distributors in that region.

Query:

SELECT *
FROM
(SELECT Distributor_ID, Frequency, REGION
FROM Distributor
WHERE Distributor_ID IN (SELECT Distributor_ID FROM Distributor WHERE (REGION =
'Jordan' OR REGION = 'Lebanon')))
ORDER BY Frequency ASC

Output:

Scenario 5:
Oureditorsinthecompanyhaverealizedthatoneofourpublicationscontainednoncredible
sources.Inordertohandlethissituation,wedecidedtoretrievetheheadline,theISSNofall
publicationsreleased on“29-NOV-2022”,and theID andnameof theemployeesthathave
worked in that publication.
Query:
SELECT E_ID
FROM Works_On
WHERE Article_ID IN (SELECT Article_ID
FROM Article
WHERE Article_Date = '29-NOV-2022

Note : The absence of output in this query is due to the lack of enough matching data in our
database.

Scenario 6:

Ancyberattackhastargetedourportalcausingaleakofourusersdata.Asacompensation,
wewanttogivealltheusersthathaveacurrentlyactiveaccountandwhosejoindateisbefore
thedateoftheattackwhichtookplacein“13-FEB-2022”,adiscountof50%byupdatingthe
price of their subscription.

Query:

UPDATE Subscription_Plan
SET Price =
CASE
WHEN Sub_num IN (SELECT Sub_num
FROM (SELECT * FROM Userk
WHERE Sub_start > '13-FEB-2022') THEN Price*0.5
ELSE Price
END
//—---------------------------------------------------
SELECT Price
FROM Subscription_Plan
WHERE Sub_num IN (SELECT Sub_num
FROM (SELECT * FROM Userk
WHERE Sub_start > '13-FEB-2022') )

Output:

Scenario 7:
Fake-Phobicdecidestorewarditshardworkingemployees.Tohelpourcompanyidentifythe
bestemployeespereverydepartment,weretrievetheemployeewiththelongestworkinghours
and the least salary, and display their salaries after a 10% raise.

Query :
SELECT *
FROM
(SELECT E_ID FROM Works_On ORDER BY W_Hours ASC)
WHERE ROWNUM <= 5
FROM Employee
Order By Salary DESC)
WHERE ROWNUM<=1) THEN Salary *1.1
END

Scenario 8:

The company wantsto analyze thearticlesand genreof publicationsthat generatedmost
interestinordertosettheappropriatefeesforfutureadvertisements.Todoso,weretrievethe
headlineofthepublicationthathadthehighestprofitintheshortestperiodoftime.Knowingthat
we have the revenue of the advertisement and the cost of the supplier.

Note : This problem is quite an interesting one, wedecided not to remove it since we believe
that with the proper help and guidance, we will be able to properly implement it. Even Though
we are able to choose another scenario, we believe that this scenario is the most challenging
and beneficial one and we aspire to fully comprehend it and implement it.

12- Normalization:
AftercompletingthePreviousphaseswearenowreadytostartthefourthandfinalphaseof
Normalization.Having createdall relations,we shouldimprove them bynormalizingthem in
accordancewithanumberofnormalforms.Inthissection,wewillnormalizeourdatabaseupto
the fourthnormalform,the Boyce-Codd NormalForm.Usingthefournormalforms,wewill
analyzeeachrelation.Aswegothroughthefirst,second,third,andfinally,BCNFnormalform,
we can see the relationship between them.
Publication :
● The Publication relation schema satisfies all conditionsof the 1NF because it has neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Publication relation schema satisfies all conditionsof the 2NF since every non prime
attribute is fully functionally dependent on the whole primary key “ ISSN ”.
● The Publication relation schema satisfies all conditionsof the 3NF because it satisfies the 2NF
and there are no non-prime attributes that are transitively dependent on the primary key “ ISSN ”.
● The Publication relation schema satisfies all conditionsof the BCNF because there exists no
functional dependency X→A where X is not a super key or A is a prime attribute and X not a
super key.

Employee:
● The Employee relation schema satisfies all conditions of the 1NF because it has neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Employee relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattribute
is fully functionally dependent on the whole primary key “ E_ID ”.
● The Employee relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
there are no non-prime attributes that are transitively dependent on the primary key “ E_ID ”.
● The Employee relation schema satisfies all conditionsof the BCNF because there exists no
● functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Department:
● The Department relation schema satisfies all conditions of the 1NF because it has neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Department relation schema satisfiesall conditions of the 2NF since every non prime
attribute is fully functionally dependent on the whole primary key “ E_ID ”.
● The Department relationschemadoesnotsatisfy3NFbecausetherearenon-primeattributesthat
aretransitivelydependentontheprimarykey“ E_ID ”,ornonprimeattribute“ Mgr_start_date ”
depending on a non prime attribute “ Mgr_ssn ”.

● The Department relation schema satisfies all conditions of the BCNF because there exists no
functional dependency X→A where X is not a super key or A is a prime attribute and X not a super
key.

Article:
● The Article relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The Article relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ Article_ID ”.
● The Article relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
there are no non-prime attributes that are transitively dependent on the primary key “ Article_ID ”.
● The Article relation schema satisfies all conditionsof the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Client:
Client:
● The Client relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The Client relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ Client_ID ”.
● The Client relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFandthere
are no non-prime attributes that are transitively dependent on the primary key “ Client_ID ”.
● The Client relation schema satisfies all conditionsof the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Advertisement :
● The Advertisement relation schema satisfies all conditions of the1NFbecauseithas neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Advertisement relationschemasatisfiesall conditionsofthe2NFsinceeverynonprime
attribute is fully functionally dependent on the whole primary key “ Ad_ID ”.
● The Advertisement relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NF
and there are no non-prime attributes that are transitively dependent on the primary key “ Ad_ID ”.
● The Advertisement relation schema satisfies all conditionsof the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

User:
● The User relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The User relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeisfully
functionally dependent on the whole primary key “ User_ID ”.
● The User relationschemadoesnot satisfy3NF becausetherearenon-primeattributesthatare
transitively dependent on the primary key “ User_ID ”, or non prime attribute
“ Subscription_Start_date ” depending on a non primeattribute “ Subscription_num ”.

● The User relation schema satisfies all conditionsof the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Subscription Plan:
● The SubscriptionPlan relationschemasatisfiesallconditionsofthe1NFbecauseithasneither
multivalued attributes nor composite attributes. All attributes are atomic.
● The SubscriptionPlan relationschemasatisfiesallconditionsofthe2NFsinceeverynonprime
attribute is fully functionally dependent on the whole primary key “ Sub_num ”.
● The SubscriptionPlan relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe
2NF and there are no non-prime attributesthat aretransitively dependentontheprimary key
“ Sub_num ”.
● The SubscriptionPlan relationschemasatisfiesallconditionsoftheBCNFbecausethereexists
nofunctionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnota
super key.

Items:
● The Items relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The Items relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ Bar_Code ”.
● The Items relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFandthere
are no non-prime attributes that are transitively dependent on the primary key “ Bar_Code ”.
● The Items relationschemasatisfiesallconditionsoftheBCNFbecausethereexistsnofunctional
dependency X→A where X is not a super key or A is a prime attribute and X not a super key.

Supplier:
● The Supplier relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The Supplier relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ Supply_No ”.
● The Supplier relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
there are no non-prime attributes that are transitively dependent on the primary key “ Supply_No ”.
● The Supplier relation schema satisfiesall conditions of the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Works on:
● The Workson relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● TheWorksonrelationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ E_ID and Article_ID ”..
● The Workson relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
therearenonon-primeattributesthataretransitivelydependentontheprimarykey“ E_IDand
Article_ID ”.
● The Works on relationschema satisfies all conditions oftheBCNF becausethereexists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Coordinates with :
● The Coordinateswith relationschemasatisfiesallconditionsofthe1NFbecauseithasneither
multivalued attributes nor composite attributes. All attributes are atomic.
● TheCoordinateswithrelationschemasatisfiesallconditionsofthe 2NFsinceeverynon
primeattribute isfully functionallydependentonthewholeprimarykey“Supply_Noand
CO_ID”.
● The Coordinateswith relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe
2NF and there are no non-prime attributesthat aretransitively dependentontheprimary key
“ Supply_No and CO_ID ”.
● The Coordinateswith relationschemasatisfiesallconditionsoftheBCNFbecausethereexistsno
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Displays:
● The Displays relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● TheDisplaysrelationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “P_ISSN and AD_ID”.
● The Displays relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
therearenonon-primeattributesthataretransitivelydependentontheprimarykey“ P_ISSNand
AD_ID ”.
● The Displays relation schema satisfies all conditions of the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Supplies:
● The Supplies relationschemasatisfiesallconditionsofthe1NFbecauseithasneithermultivalued
attributes nor composite attributes. All attributes are atomic.
● The Supplies relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattributeis
fully functionally dependent on the whole primary key “ Supply_No, Bar_Code and P_ISSN ”.
● The Supplies relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
therearenonon-primeattributesthataretransitivelydependentontheprimarykey“ Supply_No,
Bar_Code and P_ISSN”.
● The Supplies relation schema satisfies all conditions of the BCNF because there exists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Distributor:
● The Distributor relation schema satisfies all conditionsof the 1NF because it has neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Distributor relation schema satisfies all conditions of the 2NF since every non prime attribute is
fully functionally dependent on the whole primary key “ ISSN and Distributor_ID”.
● The Distributor relation schema satisfies all conditionsof the 3NF because it satisfies the 2NF and
there are no non-prime attributes that are transitively dependent on the primary key “ ISSN and
Distributor_ID”.
● The Distributor relation schema satisfies all conditionsof the BCNF because there exists no
functional dependency X→A where X is not a super key or A is a prime attribute and X not a super
key.

Dependent:
● The Dependent relation schema satisfies all conditions of the 1NF because it has neither
multivalued attributes nor composite attributes. All attributes are atomic.
● The Dependent relationschemasatisfiesallconditionsofthe2NFsinceeverynonprimeattribute
is fully functionally dependent on the whole primary key “ ID and Depend_Name ”.
● The Dependent relationschemasatisfiesallconditionsofthe3NFbecauseitsatisfiesthe2NFand
thereare no non-prime attributes that aretransitively dependent ontheprimarykey “ ID and
Depend_Name”.
● The Dependent relation schemasatisfiesall conditionsoftheBCNF becausethereexists no
functionaldependencyX→AwhereXisnotasuperkeyorAisaprimeattributeandXnotasuper
key.

Relations with no non-prime attributes:

● Do not need normalization.
13-Conclusion:
Aspartofthisproject,wedesignedtheERandadapteditbasedonfeedback.Inaddition,we
implementedthemappingalgorithmspertheEl-Masrireference,includingall 7 steps.Wealso
showcasedthemappingandhypotheticaltablestatesonourfinaldisplay.Eventually,weputall
ofourworkintorealityandimplementedthedatabaseusingOracleExpress.Alltableswere
created,differenttypesofconstraintsweredefined,thedatabasewaspopulatedandagroupof
querieswascreatedandtestedonthedatabaseaccordingly.Finallytocompletetheprojecta
clear analysis and illustration of the relation in each entity must be drawn through the
normalization of the ER and data.

Wecansafelyconcludethatcompletingthisprojectwasawonderfullearningexperiencethat
enabled us to apply and comprehend the knowledge taughtin class. In light of this, we
recognizetheimportanceofthegivenmaterialandfeelthedesireandneedtolearnmoreabout
it in order to use it in our future work.

14- References:
Belefantis, C. (2022, April 14). Newspaper-Managment-Project .GitHub.

https://github.com/Chrisbelefantis/Newspaper-Managment-Project
Connolly, T. M., & Beg, C. E. (2015). Database systems: a practical approach to design,

implementation, and management. Pearson.
Elmasri, R., & Navathe, S. (2016). Fundamentals ofdatabase systems. Seiten [Verlag Nicht

Ermittelbar.
Mullins, C. S. (2020, July). What is a DBMS? DatabaseManagement System Definition.

SearchDataManagement.
https://www.techtarget.com/searchdatamanagement/definition/database-management-syst
em
Tanvir Al Amin, M., & Zaman Ayon, I. (2015, April 13). NMS - Newspaper Management

System. Studylib.net.
https://studylib.net/doc/5622150/nms---newspaper-management-system
