# ITE130
## Branches och tillstånd ##

<img width="968" height="496" alt="image" src="https://github.com/user-attachments/assets/7336f648-65e2-426f-83d2-9a161657c99f" />
Branches är olika tillstånd av en huvudgren. Det är en separat verision, eller tillstånd, av masterbranchen som du kan arbeta på utan att det påverkar det som redan fungerar. Det kan vara bra ifall man inte vill riskera att masterbranchen ska ta skada eller ändras under tester eller expriment. Om man ör nöjd med arbetet på sin separata branch så kan man "merga" de så att det nya arbetet flyttas över till masterbranchen. 

  
## Hur man skapar och mergar branches i git ##
* Skriv ```git branch``` i ditt git program för att se branchen du redan har.
* Standard Branchen borde heta ```Master``` och vara merkerad i grönt. Se bild nedan.
<img width="873" height="84" alt="Skärmbild 2025-11-13 134935" src="https://github.com/user-attachments/assets/c5c4c5bd-e9b6-47b5-b696-98fbbd7180b8" />

* Skriv ```git branch "new_branch"```för att skapa en ny branch.
* För att göra ändringar på den nya branchen måste man först byta till den. För att byta till den nya brancehn skriv ```git checkout new_branch``
* Det borde nu gå att se längst till höger att du har bytt branch. Se bild nedan.
<img width="922" height="195" alt="Skärmbild 2025-11-13 141603" src="https://github.com/user-attachments/assets/0982d430-819b-429d-bbc1-796e42ed54b4" />

*  Nu när du är på den nya branchen kan du göra ändringar på den utan att det rör masterbranchen.
* För att byta namn skriv ```git branch --move "valfritt namn"``` Jag valde att döpa min nya branch till ```Tillstånd2```
* Det borde nu gå att se på högersidan att namnet på branchen har bytt namn. Se bild nedan. 
<img width="922" height="115" alt="Skärmbild 2025-11-13 172933" src="https://github.com/user-attachments/assets/c318b913-daa2-4fbb-baf9-953e641967c3" />

* Nu är det fritt fram att göra vad du vill med din branch utan att det påverkar masterbranchen.
* Om du är nöjd med ditt arbete på den nya branchen och vill sätta ihop den med din masterbranch måste du först byta till din masterbranch genom att skriva ```git checkout master```
* Se till att du nu befinner dig på mastebranchen.
* Skriv nu ```git merge branch_namn``` så borde den sättas ihop med masterbranchen.


## Radera branch ##

* Se först till att du befinner din på din masterbranch. 
* Om du vill ta bort din branch så ska du skriva ```git branch -d branch_namn```
