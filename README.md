# CORSIGHT v1.0 — HUNTER EDITION

```ascii
█▀▀ █▀█ █▀▄ █▀▀ ▀█▀ █▀▀ █ █ ▀█▀  
█░░ █░█ █▀▄ ▀▀█ ░█░ █░█ █▀█ ░█░ 
▀▀▀ ▀▀▀ ▀░▀ ▀▀▀ ▀▀▀ ▀▀▀ ▀ ▀ ░▀░
```


---

### One Command. Total Destruction.

```bash
python3 corsight.py -i targets.txt -t 500 -o konghq_hunt
```

**That's it.**

---

### Features (CLI GOD MODE)

- **10x faster** than any tool
- **Never hangs** — fixed all deadlocks forever
- **Smart subdomain origins** (`https://xyz123.target.com`)
- **JACKPOT sound** on HIGH findings
- **Real-time progress bar**
- **Saves JSON + clean TXT**
- **Works on 50,000+ domains**
- **Linux • Termux • Kali • Mac**

---

### Install & Run (3 seconds)

```bash
git clone https://github.com/INTELEON404/CORSIGHT.git && cd CORSIGHT
python3 corsight.py -i targets.txt
```

**Or one-liner (no save):**
```bash
python3 -c "$(curl -fsSL https://raw.githubusercontent.com/INTELEON404/CORSIGHT/main/corsight.py)" -i targets.txt -t 1000
```

---

### Usage

```bash
-i, --input     targets file (required)
-u, --url       single target
-p, --paths     paths to test (default: /,/api,/v1,/graphql,/admin)
-t, --threads   concurrency (default: 200, max: 1000)
-o, --output    output prefix (e.g. -o kong → kong.json + kong.txt)
```

**Examples:**

```bash
# Normal hunt
python3 corsight.py -i domains.txt

# MAX SPEED (Kali/Termux)
python3 corsight.py -i biglist.txt -t 800

# Kong HQ special
python3 corsight.py -i konghq.txt -t 600 -o KONGHQ_JACKPOT_2025
```

---

### Output Example

```yaml
JACKPOT! CORS VULN!
  url     → https://2293a63582c1.us.portal.konghq.tech/api
  origin  → https://abc123xyz.konghq.tech
  ACAO    → https://abc123xyz.konghq.tech
  ACAC    → true
  HIGH → EXPLOITABLE!
```

**Files created:**
```
KONGHQ_JACKPOT_2025.json
KONGHQ_JACKPOT_2025.txt
```

---

### Pro Tips

```bash
# Hunt everything
find. -name "*.txt" -exec cat {} + | sort -u > all.txt
python3 corsight.py -i all.txt -t 1000 -o FULL_HUNT
```

```bash
# Auto-recon + scan
subfinder -dL domains.txt -all -o subs.txt
python3 corsight.py -i subs.txt -t 700
```

---


### Author

**INTELEON404** — THE PENTESTER • BUG HUNTER

> "Real hackers don't click. They type."

**GitHub:** [github.com/INTELEON404](https://github.com/INTELEON404)  
**X:** [@INTELEON404](https://x.com/INTELEON404)

