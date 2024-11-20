# MCODE-Czeki

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/MOLTENEK/MCODE-Czeki-Releases/releases)
[![Minecraft](https://img.shields.io/badge/minecraft-1.18.2--1.20.x-green.svg)](https://www.minecraft.net/)
[![License](https://img.shields.io/badge/license-Custom-red.svg)](LICENSE)

## 🎥 Prezentacja

[![MCODE-Czeki Prezentacja](https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white)](https://youtu.be/twojfilm)

<div align="center">
  <a href="https://youtu.be/twojfilm">
    <img src="https://img.youtube.com/vi/TWOJ_ID_FILMU/maxresdefault.jpg" alt="MCODE-Czeki Prezentacja" style="width: 80%; max-width: 720px;">
  </a>
</div>

## ✨ Funkcje

### 🎯 Podstawowe
- Tworzenie czeków za pomocą komendy `/czek [kwota]`
- Realizacja poprzez kliknięcie PPM
- Limity kwot
- Unikalne generowane kody zabezpieczające przed duplikacją

### 🛡️ Bezpieczeństwo
- Zabezpieczenie przed duplikacją
- System uprawnień

### 📱 Interfejs
- Konfigurowalne komunikaty
- Możliwość edytowania nazwy/lore czeku
- Tytuły i wiadomości na chacie

## 🚀 Instalacja

1. Pobierz najnowszą wersję z [Releases](../../releases)
2. Umieść plik `.jar` w folderze `plugins`
3. Zainstaluj wymagane zależności
4. Uruchom/zrestartuj serwer
5. Gotowe! 🎉

## 📋 Wymagania

- Serwer: Paper/Spigot 1.18.2 - 1.20.x
- Java: 17 lub nowsza
- Wymagane pluginy:
  - [Vault](https://www.spigotmc.org/resources/vault.34315/)  (ekonomia) - **Wymagany**
  - [Essentials](https://essentialsx.net/downloads.html) - *Opcjonalny*
  - [NBT-API](https://www.spigotmc.org/resources/nbt-api.7939/) - **Wymagany**

## 🎮 Komendy

| Komenda | Uprawnienie | Opis |
|---------|-------------|------|
| `/czek <kwota>` | - | Tworzy czek na określoną kwotę |
| `/mczeki reload` | `mcode.czeki.reload` | Przeładowuje konfigurację |

## ⚙️ Konfiguracja

```yaml
# Konfiguracja pluginu MCODE-Czeki

# Ustawienia limitów
limits:
  min-amount: 1000
  max-amount: 100000

# Ustawienia czeku
check:
  name: "&a&lCzek pieniężny - ${AMOUNT}"
  lore:
    - "&8» &7Używając czeku otrzymasz na swoje"
    - "&8» &7konto &a+${AMOUNT}&7!"
    - "&7"
    - "&8» &7Wytworzył: &f{PLAYER} {DATE}"
    - "&8» &7Unikalny kod: &b{NUMBER}"
    - "&7"
    - "&8» &aKliknij PRAWYM aby wykorzystać."

# Ustawienia wiadomości
messages:
  # Wiadomości z tytułem
  check-cashed:
    message: "&7Na twoje konto zostało dodane &f${AMOUNT}$&7!"
    type: "TITLE"
  inventory-full:
    message: "&cNie masz miejsca w ekwipunku!"
    type: "TITLE"

  # Pozostałe wiadomości
  invalid-amount: "&cNieprawidłowa kwota."
  amount-must-be-greater-than-zero: "&cKwota musi być większa od zera."
  not-enough-money: "&cNie masz wystarczająco pieniędzy."
  check-issued: "&aWystawiono czek na kwotę: &e${AMOUNT}$"
  invalid-amount-range: "&cKwota musi być między &e${MIN}$ &ca &e${MAX}$&c!"
  error-creating-check: "&cWystąpił błąd podczas tworzenia czeku!"
  invalid-check: "&cTo nie jest prawidłowy czek!"
  check-already-used: "&cTen czek został już wykorzystany!"
  usage: "&fPoprawne użycie: &9{COMMAND}"
  admin-usage: "&fPoprawne użycie: &9/mczeki reload"
  no-permission: "&cNie masz uprawnień do tej komendy!"
  config-reloaded: "&aPrzeładowano &2konfigurację!"

  # Domyślny typ wiadomości dla pozostałych komunikatów
  default-message-type: "CHAT"

# Ustawienia historii transakcji
history:
  enabled: true
  limit: 1000  # Maksymalna liczba wpisów w historii

# Ustawienia debugowania
debug:
  enabled: false  # Włącz/wyłącz dodatkowe logi
  save-errors: true  # Zapisuj błędy do pliku

```

## 📊 Statystyki i Monitoring

- Historia transakcji
- Śledzenie tworzonych czeków
- Monitoring realizacji
- System debugowania

## 🤝 Wsparcie i Kontakt

Potrzebujesz pomocy? Masz propozycje? Znalazłeś błąd?
[![Discord](https://img.shields.io/badge/Discord-molt3n__-5865F2?style=for-the-badge&logo=discord&logoColor=white)](https://discord.id/1243973415908540592)
[![Email](https://img.shields.io/badge/Email-soon-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:soon)
[![Website](https://img.shields.io/badge/Website-soon-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)](https://soon)
[![GitHub Issues](https://img.shields.io/badge/GitHub_Issues-Zgłoś_błąd-181717?style=for-the-badge&logo=github&logoColor=white)](../../issues)

## 📜 Licencja

Ten plugin jest objęty [niestandardową licencją](LICENSE).
- ✅ Możesz używać plugin na swoim serwerze
- ✅ Możesz dzielić się pluginem z innymi
- ❌ Nie możesz modyfikować kodu źródłowego
- ❌ Nie możesz sprzedawać pluginu

---
*Stworzone z ❤️ przez MCODE (molt3n_)*
