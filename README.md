# GameHub-Winlator

**Obiettivo:** partire da Winlator (open source) e creare una versione con interfaccia simile a GameHub.

---

## Stato del progetto

| Fase | Stato |
|------|--------|
| Repository creato | ✅ |
| Fork di Winlator | In corso / da completare manualmente |
| UI stile GameHub | Da iniziare |
| Prima build APK | Da fare |

---

## Cosa vogliamo ottenere

- Stessa potenza di **Winlator** (esegue programmi Windows sul telefono)
- Interfaccia più moderna e pulita, ispirata a **GameHub**:
  - Schermata home con griglia di giochi/programmi
  - Card grandi con cover
  - Navigazione semplice (Home / Libreria / Impostazioni)
  - Colori scuri e aspetto da launcher di giochi

---

## Come ottenere il codice di Winlator

Il fork automatico a volte è lento. Fai così:

### Opzione A — Fork dal sito
1. Vai su: https://github.com/brunodev85/winlator
2. Clicca **Fork**
3. Scegli il tuo account `momimomi213467-art`
4. Quando è pronto, rinominalo o lavora da lì

### Opzione B — Clone locale
```bash
git clone https://github.com/brunodev85/winlator.git
cd winlator
```

Poi apri il progetto in **Android Studio**.

---

## Struttura prevista delle modifiche UI

```
app/src/main/
├─ java/.../   ← attività e fragment
├─ res/
│   ├─ layout/     ← schermate (home, library, settings)
│   ├─ drawable/   ← icone e sfondi stile GameHub
│   ├─ values/     ← colori, temi, stringhe
│   └─ menu/
└─ AndroidManifest.xml
```

### Schermate da creare / modificare
1. **Home** — griglia di giochi recenti + scorciatoie
2. **Libreria** — tutti i container / exe
3. **Dettaglio gioco** — cover grande + pulsante Play
4. **Impostazioni** — container, grafica, controlli

---

## Requisiti per compilare

- Android Studio (ultimo)
- JDK 17
- Dispositivo o emulatore Android 7.0+
- Pazienza: la prima build di Winlator può richiedere tempo

---

## Prossimi passi

1. Completare il fork di Winlator sul tuo account
2. Analizzare i layout attuali di Winlator
3. Creare un nuovo tema scuro + componenti Material/Card stile GameHub
4. Sostituire progressivamente le schermate principali
5. Generare la prima APK di test

---

## Link utili

- Winlator originale: https://github.com/brunodev85/winlator
- Releases ufficiali: https://github.com/brunodev85/winlator/releases
- Questo progetto: https://github.com/momimomi213467-art/GameHub-Winlator

---

**Nota:** Winlator è un progetto grande. Le modifiche alla UI vanno fatte con attenzione per non rompere Wine, Box64 e i driver grafici.
