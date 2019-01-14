# THEWALLETBOT manual        
Portfel kryptowalutowy oparty na komunikacji przez komunikatory (Signal, Telegram).        
## Uwagi:        
* JeĹ›li chcesz wziÄ…Ä‡ udziaĹ‚w testowaniu portfela wyĹ›lij cokolwiek na <strong><a href="https://t.me/@Walletbot_001" target="_blank">@Walletbot_001</a> (Telegram)</strong> lub znajdĹş <strong>+48607895423 na Signalu</strong>.        
* Ustaw swĂłj nick na Telegramie (jeĹ›li nie masz). DziÄ™ki temu bÄ™dziesz mĂłgĹ‚ otrzymywaÄ‡ kryptowaluty podajÄ…c innym jedynie swĂłj @nick        
* To jest testowa wersja softu. Alpha, beta czy jakkolwiek chcesz jÄ… sobie nazwaÄ‡. Jako tester bÄ™dziesz co kilka godzin dostawaÄ‡ TESTNETOWE BITCOINY. PamiÄ™taj - ich wartoĹ›Ä‡ wynosi ZERO. Inne kryptowaluty sÄ… prawdziwe wiÄ™c jednak uwaĹĽaj co robisz.        
* SzybkoĹ›Ä‡ tego portfela podczas testĂłw jest niska co wynika z wydajnoĹ›ci sprzÄ™tu. Poczekaj chwilÄ™ po wpisaniu polecenia zanim siÄ™ poddasz.        
* MoĹĽesz siÄ™ z nami kontaktowaÄ‡ na Telegramie: <strong><a href="https://t.me/thewalletbot_help" target="_blank">thewalletbot_help</a></strong> lub mailem wallet@thewalletbot.com.        
* UsĹ‚uga jest darmowa. Jedyne pĹ‚atne elementy to standardowe opĹ‚aty dla sieci transakcyjnej (fee) i ewentualnie opĹ‚ata za mieszanie monet.        
## Polecenia dla wszystkich, nie tylko dla uĹĽytkownikĂłw:        
### <strong>help [command]</strong>        
WyĹ›wietla podstawowÄ… pomoc z listÄ… komend lub szczegĂłĹ‚owy opis wskazanej komendy.        
        
### <strong>rates [coin]</strong>        
WyĹ›wietla aktualne kursy wszystkich kryptowalut obsĹ‚ugiwanych przez portfel <a href="http://thewalletbot.com/">TheWalletBot</a> lub jedynie kurs wskazanej kryptowaluty.        
przykĹ‚ady: <strong>rates | rates LTC | rates BTC</strong>        
        
### <strong>coins</strong>        
WyĹ›wietla listÄ™ kryptowalut aktualnie obsĹ‚ugiwanych  przez portfel <a href="http://thewalletbot.com/">TheWalletBot</a>.        
        
### <strong>start [coin]</strong>        
Tworzy nowy portfel dla wskazanej kryptowaluty. DomyĹ›lnie jest to bitcoin(BTC). Twoim pierwszym portfelem musi byÄ‡  portfel BTC, dopiero gdy go masz â€“ moĹĽesz inicjowaÄ‡ kolejne kryptowaluty. Dostaniesz nowy adres, ktĂłry bÄ™dzie wyĹ›wietlony wraz z qr-kodem I linkiem do blockchaina. Nie moĹĽesz w ten sposĂłb ponownie zainicjowaÄ‡ portfela â€“ jest to operacja jednorazowa. JeĹ›li chciaĹ‚byĹ› zmieniÄ‡ TwĂłj adres â€“ uĹĽyj komendy <strong>new address [coin]</strong>.        
przykĹ‚ady: <strong>start | start LTC | start BTC</strong>        
        
## Polecenia tylko dla uĹĽytkownikĂłw:        
### <strong>show [coin]</strong>        
WyĹ›wietla TwĂłj adres wskazanej kryptowaluty wraz z qr-kodem I linkiem do blockchaina. Kodu qr moĹĽesz uĹĽyÄ‡ do otrzymania pĹ‚atnoĹ›ci np. z telefonu. DomyĹ›lnÄ… kryptowalutÄ… jest BTC.        
przykĹ‚ady: <strong>show | show LTC | show BTC</strong>        
### <strong>balance [coin]</strong>        
WyĹ›wietla stan konta wskazanej kryptowaluty. JeĹ›li nie wskaĹĽesz ĹĽadnej â€“ otrzymasz liste wszystkich kryptowalut dla jakich inicjowaĹ‚eĹ› adresy.        
przykĹ‚ady: <strong>balance | balance LTC | balance BTC</strong>        
### <strong>send address amount coin</strong>        
Inicjuje wysĹ‚anie wskazanej iloĹ›ci kryptowaluty do adresata. DomyĹ›lnÄ… kryptowalutÄ… jest BTC. WartoĹ›Ä‡ transakcji musi byÄ‡ mniejsza niĹĽ stan Twojego konta. Adresat moĹĽe byÄ‡ uĹĽyty w jednej z nastÄ™pujÄ…cych wersji:        
- poprawny adres danej kryptowaluty (na przykĹ‚ad 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB),        
- nickname z Telegrama (na przykĹ‚ad  @nickname_kolegi) lub        
- numer telefonu w peĹ‚nej wersji z Signala (+446011234567). W przypadku gdy odbiorca istnieje i uĹĽywa wskazanego komunikatora - nawet jeĹ›li nie uĹĽywa portlefa TheWalletBot - otrzyma wysĹ‚ane Ĺ›rodki, a jeĹ›li to potrzebne, zaĹ‚oĹĽymy mu nowy portfel. On sam zostanie o tym poinformowany. JeĹ›li transakcja przebiegnie poprawnie - otrzymasz do niej link na blockchainie. PamiÄ™taj o fee - opĹ‚acie dla sieci transakcyjnej. Musisz mieÄ‡ wystarczajÄ…co duĹĽo Ĺ›rodkĂłw na koncie by jÄ… zapĹ‚aciÄ‡. WiÄ™c jeĹ›li chcesz przesĹ‚aÄ‡ caĹ‚Ä… wartoĹ›Ä‡ swojego adresu - uĹĽyj w poleceniu sĹ‚owa <strong>all</strong>. W takim przypadku wszystkie Ĺ›rodki zostanÄ… przesĹ‚ane a fee bÄ™dzie odjÄ™te od wysyĹ‚anej kwoty. Typowe przyĹ‚ady polecenia send to:        
<strong>send 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB 1.2        
send @NickNameOfFriend 32 LTC        
send +446011234567 all ETH</strong>        
        
### <strong>new address [coin]</strong>        
Tworzy nowy adres wskazanej kryptowaluty I przelewa na niego wszystkie Twoje Ĺ›rodki (po odjÄ™ciu fee transakcyjnego). DomyĹ›lnÄ… kryptowalutÄ… jest BTC. Operacja siÄ™ nie powiedzie, jeĹ›li na adresie nie masz wystarczajÄ…cej iloĹ›ci monet by zapĹ‚aciÄ‡ fee. JeĹ›li stan twojego adresu to 0 â€“ dostaniesz nowy adres bez ĹĽadnej transakcji przesyĹ‚ania monet â€“ czyli nie pĹ‚acisz fee.        
przykĹ‚ady: <strong>new address BTC | new address LTC</strong>        
        
### <strong>forward [coin {address | cancel}]</strong>        
WyĹ›wietla, ustawia lub likwiduje przesyĹ‚anie kryptowaluty pod wskazany adres (przekierowanie). Wymagane jest podanie nazwy kryptowaluty â€“ nie ma wartoĹ›ci domyĹ›lnej. Adresatem moĹĽe byÄ‡ tylko poprawny adres kryptowaluty. PoniĹĽej kilka typowych przykĹ‚adĂłw uĹĽycia tego polecenia wraz z opisami:        
<strong>forward</strong> â€“ wyĹ›wietla listÄ™ aktualnie ustawionych przekierowaĹ„.        
<strong>forward BTC 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB</strong> â€“ ustawia przekierowanie dla wskazanej kryptowaluty (BTC).Od tej chwili wszystkie wpĹ‚ywy na twoj adres bÄ™dÄ… przesyĹ‚ane na wskazany adres. PrzesyĹ‚anie jest realizowane co 10 minut.        
<strong>forward BTC cancel</strong> â€“ kasuje uprzednio ustawione przekierowanie dla wskazanej kryptowaluty (BTC).        
        
### <strong>mix [coin]</strong>        
Miesza Twoje monety. Nie ma domyĹ›lnej kryptowaluty. Nie kaĹĽda kryptowaluta moĹĽe byÄ‡ poddana procesowi mieszania. Mieszanie to proces anonimizacji ĹşrĂłdĹ‚a monet. W zamian za swoje monety dostaniesz inne, na nowy adres. Dzieki temu nikt nie bÄ™dzie wiedziaĹ‚ skÄ…d masz swoje Ĺ›rodki i co z nimi robisz. Proces mieszania jest pĹ‚atny â€“ w zaleĹĽnoĹ›ci od kryptowaluty kosztuje okreĹ›lony procent + fee transakcyjne. W tej chwili moĹĽliwe jest mieszanie nastÄ™pujÄ…cych kryptowalut:   
litecoin (LTC) [opĹ‚ata: 3% + opĹ‚aty transakcyjne (fee)]        
PamiÄ™taj, ĹĽe po operacji miksowania otrzymasz Ĺ›rodki na Twoim nowym adresie.        
przykĹ‚ady: <strong>mix LTC | mix BTC</strong>        
        
### <strong>history [coin] [number]</strong>        
WyĹ›wietla historiÄ™ twoich transakcji (domyĹ›lnie 10 ostatnich transakcji). JeĹ›li nie podasz nazwy kryptowaluty â€“ dostaniesz listÄ™ transakcji wszystkich kryptowalut. JeĹ›li dostÄ™pne sÄ… jakiekolwiek dodatkowe informacje o transkacji takie jak nadawca czy odbiorca, informacja, ĹĽe jest to transakcja mieszania czy przekierowania â€“ bÄ™dÄ… one rĂłwnieĹĽ wyĹ›wietlone.        
przykĹ‚ady: <strong>history | history LTC | history BTC 5</strong>        
        
## Polecenia do ustawienia opcji konta:        
        
### <strong>email [email_address]</strong>        
WyĹ›wietla lub ustawia TwĂłj adres email. MoĹĽe byÄ‡ on potrzebny do powiadomieĹ„ ale przede wszystkim do awaryjnego odzyskania konta. JeĹ›li utracisz dostÄ™p do telefonu czy samego komunikatora â€“ bÄ™dzie to jedyna droga by sie z nami skontaktowaÄ‡ i potwierdziÄ‡ swojÄ… toĹĽsamoĹ›Ä‡. Polecenie bez podania parametru wyĹ›wietla ustawiony wczeĹ›niej email. Aby zmienic email po prostu ustaw nowy.        
przykĹ‚ady: <strong>email | email your_nick@your_domain.com</strong>        
        
### <strong>fee [low | normal | high]</strong>        
WyĹ›wietla lub ustawia wysokoĹ›Ä‡ opĹ‚aty transakcyjnej (fee) dla sieci kryptowaluty. Im wiÄ™cej bÄ™dziesz pĹ‚aciĹ‚ â€“ tym szybciej Twoja transakcja zostanie zatwierdzona. Dostepne sÄ… 3 poziomy, standardowe ustawienie to normal.        
przykĹ‚ady: <strong>fee | fee low</strong>        
        
### <strong>lang [en | pl]</strong>        
WyĹ›wietla lub ustawia TwĂłj preferowany jÄ™zyk. Wszystkie polecenia zostajÄ… bez zmian â€“ po angielsku â€“ jednak opisy czy pomoc dostÄ™pna jest rĂłwnieĹĽ w innych jÄ™zykach. Polecenie bez parametru wyĹ›wieta ustawiony przez Ciebie jÄ™zyk.        
przykĹ‚ady: <strong>lang | lang en</strong>         
        
