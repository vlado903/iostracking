# iostracking

Rozpoznávání cloudově konfigurovatelných aktivit pro iOS zařízení využívající data z HealthKit frameworku.

Serverová část poskytuje REST endpoint s pravidly pro rozpoznání aktivit (např. průměr tep > 130 a zároveň počet kroků nižší než 50 každou minutu po dobu 10 minut).

Pravidla jsou uživatelsky editovatelná ve webovém prohlížeči. 

iOS klient pravidla ukládá a periodicky kontroluje, zda-li nejsou splněny podmínky pro vyvolání akce - zobrazení notifikace, zobrazení dotazníku.

Pro vyhodnocování aktivit jsou použita data z HealthKit frameworku, kam ukládají data zařízení a aplikace podporující platformu Health od Apple (např. iPhone, Apple Watch, Strava,..), se zvláštním zaměřením na data získané z Apple Watch.

Vše probíhá v reálném čase a je schopno reagovat na každodenní situace (uživatel zahájil chůzi, sportuje, atp.)
