# Murugan Trader EXE – eppadi use panradhu

## 1. GitHub la podanum
Indha folder la irukkura `desktop-app` folder + `.github` folder ah ungal repo root la copy pannunga.
(Website files (index.html, api...) kooda irukkalam, problem illa.)

## 2. EXE build
GitHub repo -> **Actions** -> **Build Windows EXE** -> **Run workflow**.
5-10 min la mudiyum. Mudinja piragu run ah open pannunga -> keezha **Artifacts** la `MuruganTrader-Setup` download pannunga (zip kulla `MuruganTrader-Setup.exe`).

Release link vennum na:  `git tag v1.0.0` then `git push --tags`  -> **Releases** page la direct download link varum. Customer ku adhe link kudukalam.

## 3. Customer side
`MuruganTrader-Setup.exe` double click -> automatic install -> Desktop shortcut + Start Menu. Vera requirement ethuvum install panna vendam.
Windows 7 SP1 / 8 / 10 / 11, 32-bit & 64-bit ellame work aagum.

## Notes
- Website URL maatha vennum na `desktop-app/main.js` la `SITE_URL` + `ALLOWED_HOSTS` maathunga.
- Electron version (22.3.27) maatha vendam – adhu dhaan Windows 7 support panra last version.
- Windows SmartScreen "Unknown publisher" warning varalam (code-signing certificate illa na). "More info -> Run anyway".
- Internet venum (website online la irukku, payment/OTP server la run aagudhu).
