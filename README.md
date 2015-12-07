# EmployeeBase
Project - by Viktor Larsson


### Grund till projekt: 
Följande länk är en kort översikt över kommande problem för byggare och byggherrar:
  http://www.svenskhandel.se/aktuellt-och-opinion/nyheter/2015/nya-regler-forsvarar-bygget/
  
Skatteverket har inför lag om att personalliggare måste införas vid alla byggplatser för att minska svartarbete.
Detta medför komplikationer för många byggföretag. 
  
Genom att komma på en smart lösning för byggare och byggherrar kan idéen faktiskt bli en realitet! 
  
Kan också vara roligt att försöka sig på något sådant här. 

Mer info :
http://www.skatteverket.se/foretagorganisationer/arbetsgivare/personalliggare/personalliggarebyggbranschen.4.7be5268414bea0646949797.html
http://www.skatteverket.se/foretagorganisationer/arbetsgivare/personalliggare/nyareglerpersonalliggare.4.3810a01c150939e893f2288.html

Ändringarna kommer införas redan 1 januari 2016. Det kommer börjas med byggbranschen men de har funderingar och planer på att införa
det för andra verksamheter också.


### TODO, förslag- 

* Server : Node.js förslagsvis. 

 *    En första sida som liksom gör reklam för produkten
 
 *    En databas för hantering av loggning. ( Kan komma att behöva implementeras en backup-bas, dono yet)
      Samt, val av databas. MySQL eller MongoDB? 
      Databasinnehåll:
      
  - Kunddatabas - organiserar kunderna. En kund är den som kommer vara huvudansvarig för en personalliggare. 
      En kund kommer vara tex chief på företaget som kommer ha X- antal anställda som ska kunnas registreras på
      portalen för att använda den digitala personalliggaren. 
          
  - "Anställda" - som har egna konton som är kopplade till en specifik kund. 
              
  - personalliggare per kund. Där man ska kunna specificiera saker och ting via ett dashboard eller
                användarportal eller liknande. 
                
  - Projekt med "sambehörighetsnummer" (eller va fan det hette). Som kopplas till kund som registrerar det. 
              
  * En enkel lösning för att kunna logga sin jobb-tid vid en anläggning. 
    - Bästa lösning vore att göra en VÄLDIGT enkel mobilapp. Tex en app där man loggar in 1 gång med sitt unika- anställningsID och 
        lösenord. Där kommer den Anställda kunna registrera sin ankomst vid en anläggning enkelt.
    - Förslag två. Att man bygger en aparat som kan läsa av( eller köper en färdig variant ) som kopplas till en viss anläggning. 
        Varje anställd kommer kunna ha ett kort som registrerar ankomst och hej då. Detta är dock mer lämpad för långtidsprojekt,
        och mindre byggföretag som har flertalet projekt per vecka är det inte särskilt "enkelt". 
        
        
  * Dashboard med information med lösanhemt och anställdas prestanda per projekt. För kunna följa hur arbetet pågår på alla                anläggningar.
  
  * Enkel kunna extrahera information från databasen i XML-format angivet av skattemyndigheten. (Finns sjukt bra node-packet för detta)     
  
    
  * Viktigast av allt är att göra hanteringen så enkel som möjlig!



### Liknande projekt : 
  http://struqtur.se/personalliggare
  http://www.templus.se/

