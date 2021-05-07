# TinderAutoLike
Auto like tinder JavaScript function - WEB PC


1 : be logged in Tinder.com and go on https://tinder.com/app/matches
2 : right click on like button, inspect element

![image](https://user-images.githubusercontent.com/18121247/117440689-ac5f0280-af34-11eb-828a-aed63c1e5a57.png)

3 : Add id="fiak" at the end of the like button

![image](https://user-images.githubusercontent.com/18121247/117440748-c39df000-af34-11eb-97e0-1cb630399f42.png)

4 : Open console
5 (optionnal) : Try by typing : document.getElementById("fiak").click(); 
If functionnal, it will like

6 : Still in console, type 
var compteur=0;

Now creating like() function :
function like(){
    console.log("Start of like function");
    document.getElementById("fiak").click();
    compteur=compteur+1;
    console.log("Like number **** " + compteur +" ****");
    console.log("end of like function");
}

Try by taping like(); (if functionnal, it will like)

7 : And now automating the function by this :

const interval3 = setInterval(function() {
   like();
 }, Math.floor(Math.random() * 1000) + 500);  // random time 500 to 1500ms);


Advice : Keep the random time to now be banned.

This is just for FUN. And BE kind with women.
