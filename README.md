# DSRacing Buttonbox Studio

Aplikacja Windows do Buttonboxa z trzema panelami 1,46″. To repozytorium udostępnia **instalatory i instrukcje**. Kod źródłowy projektu i prywatne profile użytkownika nie są publikowane.

## Pobierz i zainstaluj

**[Pobierz instalator DSRacing Studio](https://github.com/dareksteuer/dsracing-studio-releases/releases/latest/download/DSRacingStudio-Setup.exe)**

1. Pobierz plik, zamknij działające Studio i uruchom instalator.
2. Wybierz język: polski, niemiecki lub angielski, następnie **Zainstaluj**.
3. Po instalacji uruchom Studio ze skrótu na pulpicie lub w menu Start.

Link pobiera plik. Przeglądarka i Windows wymagają samodzielnego uruchomienia instalatora; nie jest to instalacja bez zgody użytkownika.

## Wydanie R102

Pakiet instalacyjny R102 zachowuje funkcje oraz interfejs Studio R100, zgodne z dotychczasowym wariantem trzech USB i panelami R098. Dlatego w interfejsie pozostaje oznaczenie R100.

- Instalacja dla bieżącego użytkownika do `%LOCALAPPDATA%\DSR\ButtonboxStudio`.
- Wykrywanie Microsoft WebView2 i instalacja brakującego składnika z oficjalnego pakietu Microsoft.
- Skróty na pulpicie i w menu Start; wpis do odinstalowania w ustawieniach Windows.
- Zachowanie danych w folderze `Dane`, kopia zastępowanych plików i wycofanie zmian przy błędzie kopiowania.
- Pomocnik czasu R074: uruchamiany przy logowaniu do Windows, bez okresowych korekt zegarów.
- Instalator **nie wgrywa firmware** i nie konfiguruje SimHuba. Mostek DLL jest dołączony do osobnej integracji.
- Eksperymentalne paczki RS485/DS3231 nie są udostępniane w tym wydaniu.

## Wymagania i weryfikacja

Windows 10/11, .NET Framework 4.6.2 lub nowszy (zalecany 4.8), Microsoft WebView2. Jeśli WebView2 nie jest zainstalowany, potrzebny jest internet.

Instalator nie ma komercyjnego podpisu cyfrowego. Windows może ostrzec o nieznanym wydawcy. Nie wyłączaj ochrony systemu; w razie blokady zachowaj dokładny komunikat. Suma SHA256 znajduje się w plikach wydania.

Sprawdzone lokalnie: 56 kontroli instalacji, zachowania profili, kopii, cofania zmian, skrótów i uruchomienia; 72 kombinacje języka, tła i trybu w natywnym WebView2. **Pełny test instalacji na drugim komputerze i test brakującego WebView2 pozostają do wykonania.** Nie wykonano nowego testu USB ani gry w ramach tej paczki.

Dziennik instalacji: `%TEMP%\DSRacing-Setup-*.log`. Dane i poprzednie wersje są zachowywane również przy odinstalowaniu.

## Deutsch

[Windows-Installer herunterladen](https://github.com/dareksteuer/dsracing-studio-releases/releases/latest/download/DSRacingStudio-Setup.exe). Datei öffnen, Sprache wählen und installieren. Studio vorher schließen. Fehlendes WebView2 wird mit Internetzugang installiert. Profile bleiben erhalten. Keine Firmware-Aktualisierung; SimHub wird separat eingerichtet. Das Programm ist nicht digital signiert.

## English

[Download the Windows installer](https://github.com/dareksteuer/dsracing-studio-releases/releases/latest/download/DSRacingStudio-Setup.exe). Open the downloaded file, choose a language and install. Close Studio first. Missing WebView2 is installed using Microsoft's bootstrapper and requires internet. Existing profiles are preserved. No firmware flashing; SimHub setup is separate. The installer is not digitally signed.

---

Zasoby interfejsu są częścią programu. Dystrybucja binarna nie zapobiega analizie ani odtwarzaniu jego działania. Znaki marek należą do ich właścicieli; aplikacja nie deklaruje współpracy z nimi.

[Dokumentacja Microsoft WebView2](https://learn.microsoft.com/en-us/microsoft-edge/webview2/concepts/distribution)
