# 💰 MCODE-Czeki

> Zaawansowany system czeków dla serwerów Minecraft

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)](https://github.com/MOLTENEK/MCODE-Czeki-Releases/releases)
[![Minecraft](https://img.shields.io/badge/minecraft-1.18.2--1.20.x-green.svg)](https://www.minecraft.net/)
[![License](https://img.shields.io/badge/license-Custom-red.svg)](LICENSE)

## ✨ Funkcje

### 🎯 Podstawowe
- Tworzenie czeków za pomocą `/czek [kwota]`
- Realizacja poprzez kliknięcie PPM
- Limity kwot (1000$ - 100000$)
- Unikalne kody zabezpieczające

### 🛡️ Bezpieczeństwo
- Zabezpieczenie przed duplikacją
- Sprawdzanie stanu konta
- Weryfikacja miejsca w ekwipunku
- System uprawnień

### 📱 Interfejs
- Nowoczesny system powiadomień
  - Tytuły na ekranie (domyślne)
  - BossBar z auto-ukrywaniem
  - Wiadomości na czacie
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
# Limity kwot
limits:
  min-amount: 1000.0
  max-amount: 100000.0

# Wygląd czeku
check:
  name: "&a&lCzek pieniężny - &e{AMOUNT}$"
  lore:
    - "&7Kliknij PPM aby zrealizować"
    - "&7Kwota: &f{AMOUNT}$"
    - "&7Wystawca: &f{PLAYER}"

# System wiadomości
messages:
  location: "TITLE"  # TITLE/BOSSBAR/CHAT
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
*Stworzone z ❤️ przez MOLTENEK*
