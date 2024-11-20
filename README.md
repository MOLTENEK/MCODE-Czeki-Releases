# MCODE-Czeki

System czeków dla serwerów Minecraft.

## Funkcje
- Tworzenie czeków za pomocą komendy `/czek [kwota]`
- Limity kwot (1000$ - 100000$)
- Realizacja czeku poprzez kliknięcie prawym przyciskiem myszy
- Automatyczny transfer pieniędzy
- Zabezpieczenia przed duplikacją

## Wymagania
- Minecraft 1.18.2 - 1.20.x
- Vault
- EssentialsX

## Instalacja
1. Pobierz najnowszą wersję z sekcji [Releases](../../releases)
2. Umieść plik .jar w folderze plugins
3. Uruchom ponownie serwer
4. Skonfiguruj plugin w pliku config.yml

## Komendy
- `/czek [kwota]` - tworzy czek na określoną kwotę
- `/mczeki reload` - przeładowuje konfigurację

## Uprawnienia
- `mcode.czeki.reload` - dostęp do komendy reload
