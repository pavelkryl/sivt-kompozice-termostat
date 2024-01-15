# Termostat

Pomocí kompozice naprogramujte termostat. Součástky/komponenty:
- **teploměr**:
  - umí vrátit aktuální teplotu v místnosti
- **spínač topení**:
  - umí vrátit stav zde je zapnuto/vypnuto
  - umí zapnout/vypnout

## Co umí

Logika, kterou bude termostat umět:
- běží a hlídá zda teplota není příliš vysoká/nízká
- pokud je nízká: sepne topení
- pokud je dostatečná: vypne topení

Z toho vyplývá konfigurace/stav termostatu, stačí nastavit v konstruktoru:
- cílová teplota na kterou se vytápí
- perioda, se kterou kontroluje teplotu

Termostat o sobě bude umět dát vědět, co schopnost to metoda:
- aktuální nastavená cílová teplota
- aktuální teplota v místnosti
- zda se topí nebo ne

## Bonusy
- naprogramujte hysterezi/setrvačnost
- dodělejte možnost měnit parametry termostatu již za běhu
  - stačí když se zohlední při dalším probuzení
  - pokud byste chtěli umět zohlednit konfiguraci hned, budete muset pracovat s thready: https://stackoverflow.com/questions/5114292/break-interrupt-a-time-sleep-in-python
- konfigurovatelná funkce, která bude umět vyhodnotit, zda se má sepnout topení nebo nikoliv
  - předávat v konstruktoru (lambda/kontrakt)

# Hodnocení
Dejte pozor zejména na:
- bez mypy errorů/warningů!
- čitelnost
- čistotu kódu
- univerzálnost: programujeme pomocí kontraktů

Možnost získat známku váhy 4.
