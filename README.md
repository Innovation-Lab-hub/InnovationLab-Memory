# InnovationLab-Memory

Layer di memoria persistente per l'**Osservatorio Innovation LAB · Engage Finance**.

Questo repository raccoglie i dati prodotti dai moduli dell'Osservatorio. È pubblico e accessibile in lettura da tutti i moduli dell'app senza autenticazione.

---

## Struttura

```
InnovationLab-Memory/
  ├─ README.md
  ├─ storico-notizie.json          ← alimentato da M1 Scout
  └─ documenti-normativi/          ← PDF normativi (alimentato da M1, letto da M3)
       └─ 2026/
            └─ [tag]-[nome].pdf
```

## File

### `storico-notizie.json`
Array di tutte le notizie validate e pubblicate da M1 Scout. Usato per deduplicazione.

```json
[
  {
    "url": "https://...",
    "titolo": "Titolo della notizia",
    "data_pubblicazione": "2026-05-19",
    "tag": "Normativa"
  }
]
```

### `documenti-normativi/`
PDF normativi scaricati durante lo scouting. Organizzati per anno.  
Convenzione di naming: `[tag]-[nome-descrittivo].pdf`  
Es: `normativa-dora-implementazione-v2.pdf`

---

*Innovation LAB · Engage Finance — maggio 2026*
