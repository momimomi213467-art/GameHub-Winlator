# GameHub-Winlator

Winlator + UI stile GameHub + build APK con **GitHub Actions**.

---

## Percorso scelto: opzione 1 (compilare Winlator con Actions)

### Realta importante

Il repo principale `brunodev85/winlator` usa **submodule** e componenti nativi pesanti.
Il codice Android vero e in:

**https://github.com/brunodev85/winlator-app**

Le release ufficiali (APK gia pronte) sono qui:
**https://github.com/brunodev85/winlator/releases**

Compilare Winlator da zero con Actions e possibile ma **difficile** (submodule, asset, librerie native). Spesso la build fallisce senza configurazione avanzata.

---

## Cosa fare da telefono (passo passo)

### 1. Fai il fork del codice app
1. Apri: https://github.com/brunodev85/winlator-app
2. Tocca **Fork**
3. Scegli il tuo account `momimomi213467-art`
4. Aspetta che compaia: `github.com/momimomi213467-art/winlator-app`

### 2. Quando il fork e pronto
Scrivimi **"fork fatto"**. A quel punto:
- collego / copio il workflow Actions nel fork
- provo a far partire la build
- se la build riesce, l APK esce in **Releases** e la scarichi dal telefono

### 3. Scaricare un APK gia pronta (senza compilare)
Se ti serve Winlator subito:
1. Vai su https://github.com/brunodev85/winlator/releases
2. Scarica l ultimo `.apk`
3. Installalo sul telefono

---

## Workflow Actions

In questo repo c e gia:
`.github/workflows/build-apk.yml`

Quando nel repo c e un progetto Gradle completo (`gradlew` + `app/`), Actions:
1. Compila l APK debug
2. La carica come Artifact
3. Crea un Release scaricabile dal telefono

---

## Limiti onesti

| Cosa | Fattibile? |
|------|------------|
| Scaricare APK ufficiale Winlator | Si, subito |
| Fork winlator-app da telefono | Si |
| Build Actions di un hub semplice | Si, affidabile |
| Build Actions di Winlator completo | Difficile, puo fallire |
| UI completa stile GameHub | Solo dopo che la build funziona + modifiche al codice |

---

## Prossimo passo

**Fai il fork di winlator-app** e scrivi `fork fatto`.

Link diretto:
https://github.com/brunodev85/winlator-app
