## Feladat: Vásárlók osztályának létrehozása

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

## Feladat: Tesztprogram (Program.cs) készítése a vásárló osztályhoz

Cél: \
Készíts egy konzol alkalmazást, amelyben a korábban létrehozott vásárlót reprezentáló osztály működését teszteled. A feladat célja, hogy a kivételkezelés, a metódusok helyes meghívása, valamint a tömbök és ciklusok használata révén ellenőrizd az osztály funkcionalitását.

**Feladatkövetelmények:**

1. **Alapüzenet megjelenítése:**
    * A program indulásakor írj ki a konzolra egy üdvözlő szöveget (például "Hello, World!").
2. **Negatív értékű inicializálás kezelése:**
    * Próbálj meg létrehozni egy olyan példányt az osztályból, ahol a kezdeti egyenleg negatív értékű.
    * Használj kivételkezelést, hogy a negatív érték miatti hibát elkapd, és jelenítsd meg a hibát a felhasználó számára.
3. **Érvényes vásárló példány létrehozása:**
    * Hozz létre egy példányt az osztályból érvényes, pozitív kezdeti egyenleggel.
    * Írd ki a példány aktuális állapotát a konzolra.
4. **Egyenleg növelésének tesztelése:**
    * Hívd meg az osztály azon funkcióját, amely egy pozitív értékkel növeli a vásárló egyenlegét.
    * Növeld az egyenleget több alkalommal különböző összegekkel.
    * Írd ki a konzolra, hogy hányszor történt az egyenleg növelése (használd a megfelelő számláló tulajdonságot).
5. **Vásárlási képesség ellenőrzése:**
    * Valósítsd meg azt a funkciót, amely ellenőrzi, hogy a vásárló elegendő egyenleggel rendelkezik-e egy adott összegű vásárlás lebonyolításához.
    * Írd ki, hogy a vásárló meg tudja-e venni a megadott értékű terméket (például egy 45 000 Ft-os monitort).
6. **Vásárlás művelete és hibakezelés:**
    * Próbálj meg végrehajtani egy vásárlást egy olyan összeggel, ami meghaladja a vásárló aktuális egyenlegét.
    * Használj kivételkezelést a hibás vásárlás elkapására, és jelenítsd meg a hibaüzenetet.
    * Ezután hajts végre egy sikeres vásárlást egy megfelelő összeggel, és írd ki a vásárlás utáni egyenleget, valamint az objektum aktuális állapotát.
7. **Több vásárló tesztelése:**
    * Hozz létre egy kollekciót (például tömböt) több vásárló példánnyal, különböző kezdő egyenlegekkel (beleértve legalább egy olyan esetet, amikor az egyenleg 0 Ft).
    * Iterálj végig a kollekción, és jelenítsd meg minden vásárló aktuális állapotát a konzolon.

**Megjegyzés:**



* Ügyelj a logikus hibakezelésre 
