Json
1.	 Sending data -  JSON.stringgify(obj)
2.	Receiving Data - JSON.parse(myJSON);
 

#Json – javascript object notation. 
# We are storage data any server with api that’s call in need   json format.  Json format is easy to quickly data fatches.  It’s necessary for development working. 


# json data are 2 type like  
1.	Json object 
2.	Json array.

# at first json object..
1.	 Mainly Json Object are including to json array..
2.	{ } that call object mean. Starting to name an call by object name.
3.	 [] – json array. 
4.	 We want to many other object in array. 




New JSON:-
Why Json:-
1.	Json mainly a text file. Such as many other data storage in Json.  Json data read and write is very easily.

2.	Json data processing is a little bit time.

3.	Json mainly working server and client relation build ..


4.	Server make a  json file  and send to client

5.	 Same to same , Client make a Json file create and send to server. 


6.	 That’s call Json is Javascript object notation..

7.	Jaavascript and JSON file are both of them declare to same object.

# Rules of Json File: 
1.	Key value and pair.
2.	Object start to – { }
3.	Every key are must declare  to quotation mark “key” 
4.	Value are not fact such as using int , string , “ value- string“, value - int

5.	New value adding to use (, koma)
6.	If any JSON file are ending don’t use to (, koma) 

Ex: {
           "name":"Uzzal",
	        "email":"uzzalcontact@gmail.com"
}

7.	JSon file are use to array now.
8.	Array’s are including to  put object.
9.	 [ ] – that is call array.
10.	Links: [ ]
11.	 When a object necessary to use 
First  start  { } 


Ex

[{
	"name":"Uzzal",
	"email":"uzzalcontact@gmail.com"
	"links" : [
	    
		  {"facebook": "https://www.facebook.com/uzzalcontact"},
		  {"linkdin": "https://www.linkedin.com/in/uzzalcontact/?originalSubdomain=bd"},
		  {"twitter": "https://twitter.com/uzzalcontact"}
	
	],
	
	"skils":["Java" , "Kotlin", "Dart", "Android", "Fluter"],
	"age": 24,
	"dept: : "CSE"
	
	
	
},



{
	"name":"Uzzal",
	"email":"uzzalcontact@gmail.com"
	"links" : [
	    
		  {"facebook": "https://www.facebook.com/uzzalcontact"},
		  {"linkdin": "https://www.linkedin.com/in/uzzalcontact/?originalSubdomain=bd"},
		  {"twitter": "https://twitter.com/uzzalcontact"}
	
	],
	
	"skils":["Java" , "Kotlin", "Dart", "Android", "Fluter"],
	"age": 24,
	"dept: : "CSE"
	
	
	
}]


Json All Tutoiral Let’s Go Chanel

How to use Android JSON Data parse:- 
1.	 Javascript object notatition.
2.	Just using to server.
3.	 Api te j data gula rakhi just format to JSON.
4.	 Easy to data face .
5.	 Json data development er jonoo essential.
6.	 JSON data are two type Json object and Json  array.
7.	Json object incuding to Json array.
8.	That’s call JSON object { }
9.	That’s call JSON array [ ].
10.	Last object don’t use to (, koma).
11.	Key and value.
12.	Key that is use to “quotation” and value is not use always quotation.
13.	Json data make to upload paid or any server fetch to api. Like  myJson website
14.	Please all of data copy and paste myJson website and click to save and you can get a api link.
15.	Api link to including in your all of data..
This is api link base of work to android programming..

Ex: 
{"studentInfo":[ -  //json array.
	{   // json object 
		"name": "Stev",
		"age": "20",
		"department": "CSE"
	},


Android studio code of
Json Fetches / Json parsing

1.	First data show of create a textfile – xml
2.	Fetch to api online so use to android userpermission internet go to manifest.
3.	We are using to http link , so we should call to http , such as we are entered Into the visit a link. 
4.	Firstly we are create a class below the oncreate method.
5.	Just class name is jsonTask with extends a AsyncTask<>

# asyncTask – asyncTask holo amder ke alada akta background thread dibe, jekhane amara http call ta korbo. And implement korte parbo.

# Android theke network a call korar jonno actually theread a use kora hoy. This is use for asyncTask.

Theread  –  aksathe onek gulo kaj kora jai.

# asyncTask<>  -  generally want to three parameter. And start to curly bracket. You can use to the depend on your datatype.  Then method doInBackground overriding to asyncTask.
# postexcute korar jonno amder j method ta projon seta holo onPostExcute() method.

6.	 doInBackground  - akonamra doInBackground ei method er maddhome amara amder http call ta korbo / network call ta korbo.

# first HttpUrlConnection variable nibo http connect korar jonno.

# api url ta rakahar jonno Url class nibo then create a object. And paste to the api url.  Then srounding korbo for network call with use to try&case.

#try&cetch – url connection Jodi kaj na hoy tahole cetch a kaj korbe..

7.	Httpconnection er maddhome url ta connect kore hobe. And url.openconnection method ti call korte hobe. Then try&cetch srounding korte hobe.and alt+enter press to cust korbo.

8.	Data gulu porte hobe ba ante hoeb ejonno jeta projon seta holo inputstream

9.	Inputstream – input stream er kaj holo api er moddhe j data gulo thakbe sei data gulo  read korte parbe ba byte korte parbe.  

10.	Inputstram er object create kore  httpurlconnection er moddhe j data gulo ache seta getInputStream korbo ..

11.	Input stream er moddhe amder byte code gulo ashes to amader jeta projon seta holo chareter gulo projon. Charateter nite hole amader BufferReader er projon.

12.	 Buffer reader er global variable declare kori. Buffer reader er object declare korlam, new(InputstreamReader) er kaj holo byte code (0,1) dara char a send korte parbe. BufferReader a ashbe. Then amara akon read korte parabo.

13.	StringBuffer nite hobe, karon BufferReader a amar line to line ashbena, e jonno line to line asar jonno StringBuffer nibo.

14.	Line gulo count korar jonno line variable declare koralm.  Liner er maddhome stringBufferReader er maddhome line by line pore StringBuffer a diye dibo.

15.	While loop create – line == buffeReader.readline != null  if null na hoy tahole se akta kaj korbe.  stringBuffer a line to line sob gulo chole ashbe..

16.	 StringBuffer.appeand(line) – appeand mane hole oi  line tai jog korbo.

17.	Return korbo stringbuffer.toString().

18.	Sobgulo line chole ashbe onPostExcute(String s) er moddhe, ki ashbe amder toString value tai. 

19.	Erpor post excute a oi string gulo amara dakhte parbo..

20.	Ter age akta kaj amra j http call gulo korsi egulo amader stop kore dite hobe. Eta korte hobe catch er pore finaly keyword use kore.   Httpurlconnection.stop();
  bufferReader.close();
  ami saina offline line gulo execute hok.
  Then alt+enter press. 
 Then try catch korte hobe default null    thakle se excute hobena.

21.	Textview ta akon set korbo s er moddhe.

22.	Ei j  jsonTaskClass  ta make korsilam eta onCreate er moddhe kono object declare korini. Ei jonno amader jeta projon seta holo, jsonTaskClass er object declare korte hobe.

23.	jsonTask  jTask = new jsonTask() then jTask.excute  korte hobe. Korle jsonTask name class ache seta excute hobe ba kaj korbe.

24.	Run korle sob gulo data chole ashbe. J gulo amder api te silo. Data fatches korte amara tahole sofol hote parsi. 

25.	Amra asole amder evabe saini amder code gulo sob aksathe chole asuk. 

26.	Amder data gulo alada alada vabe fetch korte saisi. 

27.	First nibo String file – mane holo amder puro file tai.  stringBuffer nisi sob gulo data appeand korsi StringBuffer er maddhome, r toString use korsi – data gulo convertion korar jonno.

28.	 File  variable moddhe sokol data gulo raksi, akon amder kaj holo Json object Json array egulo create korbo.

29.	 First of all amder purotai akta object. E jonno amder object tai ber korte hobe.  E jonno amder jsonObject tai use korte hobe.

30.	JsonObject er object declare kore file ta gather kore dibo. And try cetch. Then akon amara json er object er moddhe.

31.	Second kaj holo amra array object take fetch korbo.  E jonn o amara likhbo JsonArray jsonarray = fileObject.getJsonArray(“studentInfo”);

# json er object nite hobe, to object ta amder jeta seta holo  file object er moddhe fileObject.getJsonArray  - akon amder j array ta ache seta holo (“student”)

# array er moddhe j object gulo ache tar index nite hobe e jonno amake, 
JSONObject  arrayObject = jsonArray.getJSONObject(0);

JSONObject create korlam , arrayObject er moddhe jsonArray er moddhe j sob gulo data pete chai tai get koralm and index bole dilam 0, num array. 

32.	 Name, age, department ei 03 ti variable declare korte hobe.

33.	 Name, age, department e gulo app a set  korte hobe, akon ei gulor key gulo set korle amara peye jabo.

34.	Key gulo set korar jonno , first  - name akon name = sokol data arrayObject er moddhe get korbo then key ta diye dibo.

Ex: name = arrayObject.getString("name");

Then age , department are same rules.
name = arrayObject.getString("name");
age = arrayObject.getInt("age");
department = arrayObject.getString("department");


35.	Name age department return kore dibo.and sobar \n anbo akta kore.

36.	First array data gulo ashes but sokol array data gulo kintuo ashsena . amra chi sokol array data gulo ejonno amader akta loop chelate hobe and loop ti cholbe thik array length porjonto.

37.	Akon loop  ta amder jotobar cholbe totobar object gulo ber kore dibe. And must be getJsonObject er index dite hobe(i)

38.	Akta por r akta line apeand korar jonno , stringBuffer name r o akta variable declare korte hobe.

39.	 StringBuffer use kori aktar por aro akta line jano sundhor kore pai e jonno amara StringBuffer use kore thaki. 

40.	Akon amader StringBuffer er object  lastBuffer j object tir madhome appeand korte hobe – name, age,dept for loop er moddhe. 

41.	With return korte hobe amder lastBuffer ti then convert korte hobe toStirng er  maddhome.

42.	Akon amder data gulo valomoton fetch kore run korbe.



