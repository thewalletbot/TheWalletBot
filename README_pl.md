# THEWALLETBOT manual        
Portfel kryptowalutowy oparty na komunikacji przez komunikatory (Signal, Telegram).        
## Uwagi:        
* Jeśli chcesz wziąć udziałw testowaniu portfela wyślij cokolwiek na <strong><a href="https://t.me/@Walletbot_001" target="_blank">@Walletbot_001</a> (Telegram)</strong> lub znajdź <strong>+48607895423 na Signalu</strong>.        
* Ustaw swój nick na Telegramie (jeśli nie masz). Dzięki temu będziesz mógł otrzymywać kryptowaluty podając innym jedynie swój @nick        
* To jest testowa wersja softu. Alpha, beta czy jakkolwiek chcesz ją sobie nazwać. Jako tester będziesz co kilka godzin dostawać TESTNETOWE BITCOINY. Pamiętaj - ich wartość wynosi ZERO. Inne kryptowaluty są prawdziwe więc jednak uważaj co robisz.        
* Szybkość tego portfela podczas testów jest niska co wynika z wydajności sprzętu. Poczekaj chwilę po wpisaniu polecenia zanim się poddasz. Aktualnie Telegram jest znacznie szybszy niż Signal.        
* Możesz się z nami kontaktować na Telegramie: <strong><a href="https://t.me/thewalletbot_help" target="_blank">thewalletbot_help</a></strong> lub mailem wallet@thewalletbot.com.        
* Usługa jest darmowa. Jedyne płatne elementy to standardowe opłaty dla sieci transakcyjnej (fee) i ewentualnie opłata za mieszanie monet.        
## Polecenia dla wszystkich, nie tylko dla użytkowników:        
### <strong>help [command]</strong>        
Wyświetla podstawową pomoc z listą komend lub szczegółowy opis wskazanej komendy.        
        
### <strong>rates [coin]</strong>        
Wyświetla aktualne kursy wszystkich kryptowalut obsługiwanych przez portfel <a href="http://thewalletbot.com/">TheWalletBot</a> lub jedynie kurs wskazanej kryptowaluty.        
przykłady: <strong>rates | rates LTC | rates BTC</strong>        
        
### <strong>coins</strong>        
Wyświetla listę kryptowalut aktualnie obsługiwanych  przez portfel <a href="http://thewalletbot.com/">TheWalletBot</a>.        
        
### <strong>start [coin]</strong>        
Tworzy nowy portfel dla wskazanej kryptowaluty. Domyślnie jest to bitcoin(BTC). Twoim pierwszym portfelem musi być  portfel BTC, dopiero gdy go masz – możesz inicjować kolejne kryptowaluty. Dostaniesz nowy adres, który będzie wyświetlony wraz z qr-kodem I linkiem do blockchaina. Nie możesz w ten sposób ponownie zainicjować portfela – jest to operacja jednorazowa. Jeśli chciałbyś zmienić Twój adres – użyj komendy <strong>new address [coin]</strong>.        
przykłady: <strong>start | start LTC | start BTC</strong>        
        
## Polecenia tylko dla użytkowników:        
### <strong>show [coin]</strong>        
Wyświetla Twój adres wskazanej kryptowaluty wraz z qr-kodem I linkiem do blockchaina. Kodu qr możesz użyć do otrzymania płatności np. z telefonu. Domyślną kryptowalutą jest BTC.        
przykłady: <strong>show | show LTC | show BTC</strong>        
### <strong>balance [coin]</strong>        
Wyświetla stan konta wskazanej kryptowaluty. Jeśli nie wskażesz żadnej – otrzymasz liste wszystkich kryptowalut dla jakich inicjowałeś adresy.        
przykłady: <strong>balance | balance LTC | balance BTC</strong>        
### <strong>send address amount coin</strong>        
Inicjuje wysłanie wskazanej ilości kryptowaluty do adresata. Domyślną kryptowalutą jest BTC. Wartość transakcji musi być mniejsza niż stan Twojego konta. Adresat może być użyty w jednej z następujących wersji:        
- poprawny adres danej kryptowaluty (na przykład 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB),        
- nickname z Telegrama (na przykład  @nickname_kolegi) lub        
- numer telefonu w pełnej wersji z Signala (+446011234567). W przypadku gdy odbiorca istnieje i używa wskazanego komunikatora - nawet jeśli nie używa portlefa TheWalletBot - otrzyma wysłane środki, a jeśli to potrzebne, założymy mu nowy portfel. On sam zostanie o tym poinformowany. Jeśli transakcja przebiegnie poprawnie - otrzymasz do niej link na blockchainie. Pamiętaj o fee - opłacie dla sieci transakcyjnej. Musisz mieć wystarczająco dużo środków na koncie by ją zapłacić. Więc jeśli chcesz przesłać całą wartość swojego adresu - użyj w poleceniu słowa <strong>all</strong>. W takim przypadku wszystkie środki zostaną przesłane a fee będzie odjęte od wysyłanej kwoty. Typowe przyłady polecenia send to:        
<strong>send 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB 1.2        
send @NickNameOfFriend 32 LTC        
send +446011234567 all ETH</strong>        
        
### <strong>new address [coin]</strong>        
Tworzy nowy adres wskazanej kryptowaluty I przelewa na niego wszystkie Twoje środki (po odjęciu fee transakcyjnego). Domyślną kryptowalutą jest BTC. Operacja się nie powiedzie, jeśli na adresie nie masz wystarczającej ilości monet by zapłacić fee. Jeśli stan twojego adresu to 0 – dostaniesz nowy adres bez żadnej transakcji przesyłania monet – czyli nie płacisz fee.        
przykłady: <strong>new address BTC | new address LTC</strong>        
        
### <strong>forward [coin {address | cancel}]</strong>        
Wyświetla, ustawia lub likwiduje przesyłanie kryptowaluty pod wskazany adres (przekierowanie). Wymagane jest podanie nazwy kryptowaluty – nie ma wartości domyślnej. Adresatem może być tylko poprawny adres kryptowaluty. Poniżej kilka typowych przykładów użycia tego polecenia wraz z opisami:        
<strong>forward</strong> – wyświetla listę aktualnie ustawionych przekierowań.        
<strong>forward BTC 3D5g41AUezCr6cqZZCUykUKpK4YdA695fB</strong> – ustawia przekierowanie dla wskazanej kryptowaluty (BTC).Od tej chwili wszystkie wpływy na twoj adres będą przesyłane na wskazany adres. Przesyłanie jest realizowane co 10 minut.        
<strong>forward BTC cancel</strong> – kasuje uprzednio ustawione przekierowanie dla wskazanej kryptowaluty (BTC).        
        
### <strong>mix [coin]</strong>        
Miesza Twoje monety. Nie ma domyślnej kryptowaluty. Nie każda kryptowaluta może być poddana procesowi mieszania. Mieszanie to proces anonimizacji źródła monet. W zamian za swoje monety dostaniesz inne, na nowy adres. Dzieki temu nikt nie będzie wiedział skąd masz swoje środki i co z nimi robisz. Proces mieszania jest płatny – w zależności od kryptowaluty kosztuje określony procent + fee transakcyjne. W tej chwili możliwe jest mieszanie następujących kryptowalut:   
litecoin (LTC) [opłata: 3% + opłaty transakcyjne (fee)]        
Pamiętaj, że po operacji miksowania otrzymasz środki na Twoim nowym adresie.        
przykłady: <strong>mix LTC | mix BTC</strong>        
        
### <strong>history [coin] [number]</strong>        
Wyświetla historię twoich transakcji (domyślnie 10 ostatnich transakcji). Jeśli nie podasz nazwy kryptowaluty – dostaniesz listę transakcji wszystkich kryptowalut. Jeśli dostępne są jakiekolwiek dodatkowe informacje o transkacji takie jak nadawca czy odbiorca, informacja, że jest to transakcja mieszania czy przekierowania – będą one również wyświetlone.        
przykłady: <strong>history | history LTC | history BTC 5</strong>        
        
## Polecenia do ustawienia opcji konta:        
        
### <strong>email [email_address]</strong>        
Wyświetla lub ustawia Twój adres email. Może być on potrzebny do powiadomień ale przede wszystkim do awaryjnego odzyskania konta. Jeśli utracisz dostęp do telefonu czy samego komunikatora – będzie to jedyna droga by sie z nami skontaktować i potwierdzić swoją tożsamość. Polecenie bez podania parametru wyświetla ustawiony wcześniej email. Aby zmienic email po prostu ustaw nowy.        
przykłady: <strong>email | email your_nick@your_domain.com</strong>        
        
### <strong>fee [low | normal | high]</strong>        
Wyświetla lub ustawia wysokość opłaty transakcyjnej (fee) dla sieci kryptowaluty. Im więcej będziesz płacił – tym szybciej Twoja transakcja zostanie zatwierdzona. Dostepne są 3 poziomy, standardowe ustawienie to normal.        
przykłady: <strong>fee | fee low</strong>        
        
### <strong>lang [en | pl]</strong>        
Wyświetla lub ustawia Twój preferowany język. Wszystkie polecenia zostają bez zmian – po angielsku – jednak opisy czy pomoc dostępna jest również w innych językach. Polecenie bez parametru wyświeta ustawiony przez Ciebie język.        
przykłady: <strong>lang | lang en</strong>         
        
