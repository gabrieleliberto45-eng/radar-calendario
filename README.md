# radar-calendario

Copia del calendario economico della settimana di ForexFactory, aggiornata ogni ora da GitHub Actions.

Il bot Telegram **Radar XAU** (Cloudflare Worker `radar-oro`) legge `calendario.json` da qui invece di
chiamare ForexFactory direttamente, perché ForexFactory respinge le richieste che arrivano dai server Cloudflare.

- Script: `.github/workflows/calendario.yml` (ogni ora al minuto 17, oppure a mano da Actions → Calendario → Run workflow)
- Dati: `calendario.json`, lo stesso formato di `https://nfs.faireconomy.media/ff_calendar_thisweek.json`
