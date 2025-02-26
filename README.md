**Feladat: Vásárlói Osztály Létrehozása**

*Cél*: 
**Hozz létre egy olyan osztályt, amely egy vásárlót (ügyfelet) reprezentál, és képes kezelni a vásárló egyenlegét, valamint nyomon követi az egyenleg növelésének számát.**

**Követelmények:**

1. **Konstruktor és Inicializálás:**
    * Az osztály konstruktorának fogadnia kell legalább három bemeneti értéket: a vásárló neve, egyértelmű azonosításra szolgáló adat (pl. e-mail cím) és egy induló pénzösszeg.
    * Az induló pénzösszeg nem lehet negatív; ha mégis negatív értéket kap, akkor a konstruktor dobjon megfelelő kivételt.
2. **Adattagok és Tulajdonságok:**
    * **Név:** Hozz létre egy olyan tulajdonságot vagy mezőt, amely a vásárló nevét tárolja. Ez legyen kívülről olvasható és módosítható.
    * **Azonosító (pl. e-mail):** Készíts egy olyan tulajdonságot, amely az ügyfél egyedi azonosítóját tárolja. Ez a tulajdonság csak olvasható legyen kívülről.
    * **Egyenleg:** Az egyenleget tároló adattag legyen kívülről csak olvasható, azonban az osztályon belül módosítható.
    * **Növelés Számláló:** Valósíts meg egy olyan számlálót, amely azt mutatja, hogy hányszor történt az egyenleg növelése. Ennek a tulajdonságnak a külső módosítása ne legyen engedélyezett.
3. **Funkciók (Metódusok):**
    * **Egyenleg Növelése:**
        * Készíts egy olyan metódust, amely egy pozitív összeggel növeli az egyenleget.
        * A metódusnak növelnie kell a számláló értékét is, amely azt követi, hányszor történt növelés.
        * Ha a bemeneti összeg nem pozitív, a metódus dobjon egy kivételt.
    * **Egyenleg Ellenőrzése Vásárláshoz:**
        * Valósíts meg egy olyan funkciót, amely ellenőrzi, hogy a vásárló rendelkezik-e elegendő egyenleggel egy adott vásárlási összeg fedezéséhez.
        * A visszatérési érték legyen logikai típusú (igaz/hamis).
    * **Vásárlás Lebonyolítása:**
        * Hozz létre egy metódust, amely egy vásárlás műveletét végzi el.
        * Először ellenőrizze, hogy a vásárlás értéke pozitív; ha nem, dobjon kivételt.
        * Ezután ellenőrizze, hogy az aktuális egyenleg fedezi-e a vásárlás összegét. Ha nincs elegendő fedezet, szintén megfelelő kivételt kell dobni.
        * Ha minden feltétel teljesül, csökkentse az egyenleget a vásárlás összegével.
4. **Objektum Állapotának Megjelenítése:**
    * Valósíts meg egy olyan metódust, amely visszaad egy szöveges leírást az objektum aktuális állapotáról, például a vásárló neve, azonosítója és aktuális egyenlege.

**Megjegyzések:**

* Ügyelj arra, hogy a kivételkezelés logikus és következetes legyen, valamint a kód átláthatóan és karbantarthatóan legyen felépítve.
