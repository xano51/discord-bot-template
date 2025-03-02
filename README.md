# 🎉 Szablon Bota Discord – **Najnowsza wersja Discord.js**

![Szablon Bota Discord](https://iili.io/32P6GqJ.png)  
![Przykładowy Embed](https://iili.io/32PsAgf.png)  

---

## ⚡ Funkcje  
✔️ **Obsługa najnowszej wersji Node.js**  
✔️ **Konfigurowalny `config.js`**  
✔️ **Moduł `welcome.js` – automatyczne wiadomości powitalne**  
✔️ **Obsługa `Intents` – poprawne działanie bota**  
✔️ **Łatwa instalacja i konfiguracja**  

---

## 🔧 **Konfiguracja i Instalacja**  
### 🛠️ **1. Wymagania**  
Przed rozpoczęciem upewnij się, że masz zainstalowane:  
- 📌 **Node.js (najnowsza wersja)** → [Pobierz tutaj](https://nodejs.org/)  
- 📌 **Discord Developer Portal** → [Zarejestruj bota](https://discord.com/developers/applications)  

Uruchom poniższe komendy w **CMD/PowerShell**, aby upewnić się, że masz wszystko gotowe:  
```sh
node -v            # Sprawdzenie wersji Node.js
npm -v             # Sprawdzenie wersji npm
git --version      # Sprawdzenie wersji Git (jeśli używasz)
```

### 🔑 **2. Ustawienia uprawnień (`Intents`)**  
Aby bot działał poprawnie, musisz włączyć odpowiednie uprawnienia:  

1. 🔗 Przejdź do **[Discord Developer Portal](https://discord.com/developers/applications)**  
2. 🔍 Wybierz swojego bota  
3. ⚙️ Przejdź do zakładki **Bot**  
4. ✅ W sekcji **Privileged Gateway Intents** **włącz**:  
   - `PRESENCE INTENT`  
   - `SERVER MEMBERS INTENT`  
   - `MESSAGE CONTENT INTENT`  

### 📦 **3. Instalacja zależności**  
Pobierz repozytorium i zainstaluj wymagane moduły:  
```sh
npm install 
```

## Config Bot
module.exports = { 
    token: "TWÓJ_TOKEN_BOTA",
    guildId: "ID_TWOJEGO_SERWERA",
    welcome: {
        channelId: "ID_KANAŁU_POWITALNEGO",
        embed: {
            color: "#ff0000",
            title: "NAZWA_SERWERA",
            description: "Cześć, {user}! 🎉\nMiło Cię widzieć na **NAZWA_SERWERA!**\n\n**Obecnie mamy {memberCount} członków!**",
            fields: [
                {
                    name: "👤 Użytkownik",
                    value: "{user}",
                    inline: true
                },
                {
                    name: "📅 Data dołączenia",
                    value: "{joinDate}",
                    inline: true
                }
            ],
            thumbnail: true,
            timestamp: true
        }
    }
};

! Jeśli chcesz aby bot działał w tle użyj
```sh
npm install -g pm2
pm2 start index.js --name "DiscordBot"
pm2 save
```
