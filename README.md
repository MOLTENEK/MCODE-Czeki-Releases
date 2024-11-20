# 💰 MCODE-Czeki

> Plugin na czeki

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/MOLTENEK/MCODE-Czeki-Releases/releases)
[![Minecraft](https://img.shields.io/badge/minecraft-1.18.2--1.20.x-green.svg)](https://www.minecraft.net/)
[![License](https://img.shields.io/badge/license-Custom-red.svg)](LICENSE)

## ✨ Funkcje

### 🎯 Podstawowe
- Tworzenie czeków za pomocą `/czek [kwota]`
- Realizacja poprzez kliknięcie PPM
- Limity kwot
- Unikalne kody zabezpieczające przed duplikacją

### 🛡️ Bezpieczeństwo
- Zabezpieczenie przed duplikacją
- Sprawdzanie stanu konta
- Weryfikacja miejsca w ekwipunku
- System uprawnień

### 📱 Interfejs
- Konfigurowalne komunikaty

## 🚀 Instalacja

1. Pobierz najnowszą wersję z [Releases](../../releases)
2. Umieść plik `.jar` w folderze `plugins`
3. Zainstaluj wymagane zależności
4. Uruchom/zrestartuj serwer
5. Gotowe! 🎉

## 📋 Wymagania

- Serwer: Paper/Spigot 1.18.2 - 1.20.x
- Java: 17 lub nowsza
- Zależności:
  - Vault (ekonomia)
  - EssentialsX

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
    - "&8» &7konto &a+{AMOUNT}$&7!"
    - "&7"
    - "&8» &7Wytworzył: &f{PLAYER} {DATE}"
    - "&8» &7Unikalny kod: &b{NUMBER}"
    - "&7"
    - "&8» &aKliknij PRAWYM aby wykorzystać."

# Ustawienia wiadomości
messages:
  invalid-amount: "&cNieprawidłowa kwota."
  amount-must-be-greater-than-zero: "&cKwota musi być większa od zera."
  not-enough-money: "&cNie masz wystarczająco pieniędzy."
  check-issued: "&aWystawiono czek na kwotę: &e{AMOUNT} $"
  check-cashed: "&7Na twoje konto zostało dodane &f${AMOUNT}&7!"
  inventory-full: "&cNie masz miejsca w ekwipunku!"
  message-location: "TITLE" # CHAT/BOSSBAR/TITLE

# Ustawienia historii transakcji
history:
  enabled: true

```

## 📊 Statystyki

- Historia transakcji
- Śledzenie wystawionych czeków
- Monitoring realizacji

## 🤝 Wsparcie

Potrzebujesz pomocy? Masz propozycje?
- 📧 Kontakt: [Discord](https://discord.gg/twojserwer)
- 🐛 Zgłoś błąd: [GitHub Issues](../../issues)

## 📜 Licencja

Ten plugin jest objęty [niestandardową licencją](LICENSE).
- ✅ Możesz używać plugin na swoim serwerze
- ✅ Możesz dzielić się pluginem z innymi
- ❌ Nie możesz modyfikować kodu źródłowego
- ❌ Nie możesz sprzedawać pluginu

---
*Stworzone z ❤️ przez MCODE (molt3n_)*
