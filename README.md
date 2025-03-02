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
- node -v            # Sprawdzenie wersji Node.js
- npm -v             # Sprawdzenie wersji npm
- git --version      # Sprawdzenie wersji Git (jeśli używasz)

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
---

- npm install -g pm2  # Instalacja PM2
- pm2 start index.js --name "DiscordBot"  # Uruchomienie bota w tle
- pm2 save  # Zapisanie ustawień PM2
- pm2 logs  # Podgląd logów bota
- pm2 list  # Lista wszystkich uruchomionych procesów
