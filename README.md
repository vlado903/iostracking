# iostracking

Rozpoznávání cloudově konfigurovatelných aktivit pro iOS zařízení využívající data z HealthKit frameworku.

Serverová část poskytuje REST endpoint s pravidly pro rozpoznání aktivit (např. průměr tep > 130 a zároveň počet kroků nižší než 50 každou minutu po dobu 10 minut).

Pravidla jsou uživatelsky editovatelná ve webovém prohlížeči. 

iOS klient pravidla ukládá a periodicky kontroluje, zda-li nejsou splněny podmínky pro vyvolání akce - zobrazení notifikace, zobrazení dotazníku.

Vše probíhá v reálném čase a je schopno reagovat na každodenní situace (uživatel zahájil chůzi, sportuje, atp.)
