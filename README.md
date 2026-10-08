# RollerBot for Rollercoin

<p align="center">
  <b>Automated control and optimization tool.</b>
</p>

---

## 🇩🇪 Installation & Anleitung

1. **Herunterladen:**
   * Gehe in die [Releases](https://github.com/playmailhd-droid/RollerBot/releases)-Sektion dieses Repositories.
   * Lade die aktuelle **`RollerBot.zip`** herunter.
2. **Entpacken:**
   * Entpacke die heruntergeladene ZIP-Datei in einen Ordner deiner Wahl auf deinem PC.
3. **Starten:**
   * Starte die **`RollerBot.exe`** direkt aus dem Ordner. Alle Konfigurationen und Daten bleiben lokal auf deinem System.

### 🔒 Lokale Datenspeicherung (Datenschutz)
Der Bot speichert alle Einstellungen, Profile und Sitzungsdaten ausschließlich lokal im selben Verzeichnis auf deinem PC. Hier ein Auszug aus dem Code, der zeigt, wie Profile und Daten lokal geladen werden:

```python
import os

# Speichert alle Daten lokal im Ordner des Bots
LOCAL_DATA_DIR = os.path.join(os.getcwd(), "user_data")
os.makedirs(LOCAL_DATA_DIR, exist_ok=True)

# Beispiel für lokale Chrome-Profile / Einstellungen
CHROME_PROFILE_PATH = os.path.join(LOCAL_DATA_DIR, "chrome_profile")
