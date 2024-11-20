# MCODE-Czeki

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
- Customowe nazwy i lore czeków
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
- Zależności:
  - Vault (ekonomia)
  - NBT-API

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
```

## 📊 Statystyki i Monitoring

- Historia transakcji
- Śledzenie tworzonych czeków
- Monitoring realizacji
- System debugowania

## 🤝 Wsparcie i Kontakt

Potrzebujesz pomocy? Masz propozycje? Znalazłeś błąd?
- 💬 Discord: molt3n_
- 📧 Email: soon
- 🌐 Website: soon
- 🐛 Zgłoś błąd: [GitHub Issues](../../issues)

## 📜 Licencja

Ten plugin jest objęty [niestandardową licencją](LICENSE).
- ✅ Możesz używać plugin na swoim serwerze
- ✅ Możesz dzielić się pluginem z innymi
- ❌ Nie możesz modyfikować kodu źródłowego
- ❌ Nie możesz sprzedawać pluginu

---
*Stworzone z ❤️ przez MCODE (molt3n_)*
