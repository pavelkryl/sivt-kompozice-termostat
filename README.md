# Termostat

Pomocí kompozice naprogramujte termostat. Součástky/komponenty:
- teploměr:
  - umí vrátit aktuální teplotu v místnosti
- spínač topení:
  - umí vrátit stav zde je zapnuto/vypnuto
  - umí zapnout/vypnout

Logika, kterou bude termostat umět:
- běží a hlídá zda teplota není příliš vysoká/nízká
- pokud je nízká: sepne topení
- pokud je dostatečná: vypne topení

Z toho vyplývá konfigurace/stav termostatu:
- cílová teplota
- perioda, se kterou kontroluje teplotu