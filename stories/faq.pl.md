<!-- 
.. title: Często Zadawane Pytania
.. slug: faq
.. date: 2016-10-03 05:16:01 UTC-05:00
.. tags: 
.. category: 
.. link: 
.. description: 
.. type: text
-->

-   [Gdzie mogę znaleźć najnowszą wersję TW Blue?](#download)
-   [Jak często wydawane są nowe wersje?](#new_versions)
-   [Po zainstalowaniu aktualizacji TW Blue, program nie chce się uruchomić. Co w tej sytuacji
    zrobić?](#update_issues)
-   [Korzystam też z innego klienta Twittera, który posiada ukryty interfejs.
    Czy mogę używać go jednocześnie z ukrytym interfejsem
    TW Blue?](#multiple_hidden_windows)
-   [Czy da się wymusić aktualizację buforów
    osi czasu?](#updating_buffers)
-   [Czy mogę używać funkcji tłumaczenia w TW Blue do porozumiewania się
    z ludźmi z za granicy?](#translating)
-   [Czy mogę obsługiwać za pomocą TW Blue
    więcej niż jedno konto na Twitterze?](#more_than_one_account)
-   [Mam klucz API dla Sndup, ale moje pliki audio nie chcą się załadować,
    nawet jeżeli umieszczam je w oknie ustawień. Dlaczego tak się dzieje?](#api_key)
-   [Chcę pomagać w rozwijaniu programu. Jak mogę zaangażować się
    w projekt?](#help)

Gdzie mogę znaleźć najnowszą wersję TW Blue? {#download}
-----------------------------------------------

Najnowszą wersję programu można zawsze pobrać ze
[strony pobierania.](download.en.html) Dostępna jest tam odpowiednia
wersja dla każdej architektury systemu(32 i 64-bitowej). Należy
podkreślić, że program automatycznie sprawdza, czy dostępna jest nowa wersja. Jeżeli został
zainstalowany na Twoim komputerze, otrzymasz powiadomienie o nowej
dostępnej wersji. Zalecamy korzystać z automatycznej aktualizacji programu,
bo jest to niezwykle prosty proces. Wystarczy nacisnąć przycisk “Tak” w oknie
dialogowym powiadomienia o aktualizacji. Program pobierze nową wersję i
automatycznie ją zainstaluje.

Jak często wydawane są nowe wersje? {#new_versions}
------------------------------------

W początkowej fazie rozwoju TW Blue, nowa wersja była
wydawana co sobotę. Z czasem, nasz program stawał się coraz bardziej zaawansowany,
a w konsekwencji, jego kod coraz bardziej skomplikowany. Nie dało się już
publikować aktualizacji co tydzień. Dlatego, obecnie
nie ma stałego planu wydawania nowych wersji. Chcielibyśmy się upewnić, że
nowe funkcje działają tak jak powinny w ramach każdej aktualizacji i że nie pojawiają się
nieoczekiwane błędy. Warto śledzić nasze konto na Twitterze
[@tw\_blue2](https://twitter.com/tw_blue2) aby otrzymywać najświeższe informacje o
najnowszej dostępnej wersji. Ponadto, sam program
powiadomi Cię o zmianach.

Po zainstalowaniu aktualizacji TW Blue, program nie chce się uruchomić. Co w tej sytuacji zrobić? {#update_issues}
---------------------------------------------------------------------

Jeżeli TW Blue nie uruchamia się po zainstalowaniu aktualizacji, spróbuj wykonać następujące czynności:

-   Jeszcze raz pobierz nową wersję ze strony programu.
-   Potem wypakuj ją do folderu, w którego nazwie nie ma liter z
    akcentem. Folder ten powinien być pusty. Należy go też oddzielić od 
    tego, który zawiera wadliwą wersję programu.
-   Następnie, skopiuj folder config z niedziałającej wersji
    do folderu, który zawiera nową kopię programu.
-   Teraz spróbuj uruchomić TW Blue.
-   Jeżeli program nadal się nie uruchamia, usuń folder config i powtórz
    cały proces. Klient poprosi o autoryzację przez
    stronę Twittera.
-   Jeżeli nic nie pomoże, wypełnij raport o błędach i dołącz do niego
    zawartość następujących plików: logs/tracebacks.log, logs/debug.log
    oraz logs/error.log.

Korzystam też z innego klienta Twittera, który posiada ukryty interfejs. Czy mogę używać go jednocześnie z ukrytym interfejsem TW Blue? {#multiple_hidden_windows}
-----------------------------------------------------------------------------------------------------------------------------------

Nie, ponieważ oba te programy mają wiele wspólnych cech,
które się wykluczają. Jeżeli dwa programy z ukrytym interfejsem są uruchomione jednocześnie,
skróty klawiszowe drugiego ukrytego klienta zastępują skróty
pierwszego. Pierwszy klient staje się bezużyteczny i trzeba zabić
jego proces.

Czy da się wymusić aktualizację buforów osi czasu? {#updating_buffers}
---------------------------------------------------

Najprościej mówiąc, Nie da się. Nasz program
działa inaczej niż większość klientów Twittera, które pobierają nowe
tweety co pewien czas.

Po uruchomieniu TW Blue, wszystkie tweety pobierają się automatycznie, a program
potwierdza to komunikatem “Gotowe" i odpowiednim dźwiękiem. Od tego
momentu, nowe tweety, wzmianki, wiadomości prywatne, czy prośby o
śledzenie, które pojawią się na Twoim koncie, zostaną natychmiast rozpoznane przez TW
Blue. Jeżeli dostęp do internetu zostanie przerwany, program ponownie połączy się
z Twitterem i pobierze wszystkie brakujące tweety, kiedy
Internet będzie znów dostępny. Wszystkie wyżej opisane działania odbywają się w czasie rzeczywistym.
Nie ma zatem potrzeby wymuszania aktualizacji.

Czy mogę używać funkcji tłumaczenia w TW Blue do porozumiewania się z ludźmi z zagranicy? {#translating}
--------------------------------------------------------------------------------------------

Nie. tłumaczenia są dostarczane przez [Google
Translate](http://translate.google.com) którego twórcy sami podkreślają, że
tłumaczenia maszynowe nie dorównują tym zrobionym przez człowieka pod względem dokładności.
Oczywiście, decyzja należy do użytkownika. Jeżeli
uważasz, że tłumaczenia Google są wystarczające do tego,
co chcesz osiągnąć, to oczywiście możesz ich użyć.

Czy mogę obsługiwać za pomocą TW Blue więcej niż jedno konto na Twitterze? {#more_than_one_account}
-----------------------------------------------------

Na chwilę obecną, nie jest to wspierane. Można natomiast zainstalować oddzielną
kopię TW Blue w innym folderze i skonfigurować ją na
potrzeby drugiego konta. Tworzą się wtedy dwie instancje programu,
każda w oddzielnym oknie. Pamiętaj jednak, że ukryty interfejs
można aktywować tylko w jednej z tych instancji. Upewnij się również,
że żaden inny uruchomiony program
nie używa tych samych skrótów klawiszowych co tryb ukryty TW Blue.

Mam klucz API dla Sndup umieszczony w oknie ustawień TW Blue, ale moje pliki audio nadal nie chcą się załadować. Dlaczego tak się dzieje? {#api_key}
-----------------------------------------------------------------------------------------------------------------------------

Sprawdź następujące rzeczy:

1.  TW Blue może wysyłać pliki przedstawiając się jako niezarejestrowany użytkownik.
2.  Upewnij się, że klucz API w oknie ustawień TW Blue jest
    dokładnie taki sam jak ten na Twoim profilu na
    [SndUp.](http://sndup.net) sprawdź dokładnie, czy w kluczu nie zostały
    przez pomyłkę spacje lub znaki nowego wiersza.

Jeśli po wykonaniu powyższych czynności nadal masz te same
problemy, poinformuj nas o tym przez opcję “Zgłoś Błąd w menu
Pomoc.

Chcę pomagać w rozwijaniu programu. Jak mogę zaangażować się w projekt? {#help}
----------------------------------------------------------------------

Jeśli lubisz używać TW Blue i chcesz pomóc w jego ulepszaniu, znajdziesz
tu wiele do zrobienia. Doceniamy każdą pomoc. Poniżej znajduje się
kilka sugestii, jak pomagać w rozwoju TW Blue:

-   Zgłaszaj wszelkie zauważone błędy w zachowaniu aplikacji
    na platformie, której używasz. Wystarczy użyć opcji “Zgłoś
    Błąd" w menu Pomoc. Podaj swoje dane kontaktowe.
    Odezwiemy się do Ciebie i poprosimy o dokładne informacje na temat zgłoszonego błędu.
-   Będziemy też wdzięczni za wsparcie pieniężne w dowolnej kwocie. Można go udzielić poprzez
    naszą [stronę wsparcia.](donate.en.html) Pozwoli nam to poświęcić więcej czasu
    i energii na rozwój TW Blue.
-   Jeśli podoba Ci się ta aplikacja, możesz pomagać w jej rozpowszechnianiu polecając
    ją swoim znajomym na portalach społecznościowych.
-   Jeśli prowadzisz własną stronę internetową lub bloga, będzie wspaniale,
    jeśli napiszesz parę słów o naszym programie. Nowe pomysły i
    konstruktywną krytykę przyjmujemy z otwartymi ramionami.
-   Jeżeli posługujesz się biegle językami obcymi i zechcesz pomóc w udostępnianiu
    TW Blue ludziom na całym świecie,
    napisz do nas na [info@twblue.com.mx](info@twblue.com.mx) i prześlij
    swoje tłumaczenie.
-   Jeżeli programujesz w [Pythonie](http://python.org) and [WX
    Python](http://wxpython.org) lub w innych językach programowania i
    interesuje cię pomoc w rozwijaniu TW Blue,
    skontaktuj się z nami i zobaczymy, co da się zrobić.