# 🌙 Dreamscapes — Neural Style Transfer

## Trasformare immagini reali in visioni oniriche con Computer Vision

Questo progetto esplora il confine tra realtà e immaginazione utilizzando il **Neural Style Transfer**: una tecnica di Computer Vision che combina la struttura di un’immagine (contenuto) con colori e texture di un’altra (stile), generando una reinterpretazione visiva “da sogno”.

---

## 🎯 Obiettivo

- Generare una versione **onirica e colorata** di un’immagine reale
- Mantenere una struttura riconoscibile (equilibrio tra contenuto e stile)
- Documentare il processo con notebook commentato e visualizzazioni finali

---

## 🧠 Cos’è il Neural Style Transfer (in breve)

Il Neural Style Transfer combina:

- **Content image** → struttura, forme, composizione (la “realtà”)
- **Style image** → colori, texture, pattern (la “dimensione onirica”)

L’ottimizzazione bilancia due componenti:

- **Content loss**: preserva la struttura del contenuto
- **Style loss**: trasferisce lo stile tramite *Gram Matrix* delle feature

---

## 🧪 Metodologia

1. Caricamento e preprocessing delle immagini (PIL + torchvision)
2. Estrazione feature con rete **VGG19** pre-addestrata
3. Definizione di **ContentLoss** e **StyleLoss**
4. Ottimizzazione dell’immagine di input (LBFGS)
5. Output finale e interpretazione qualitativa

---

## 🛠️ Tecnologie utilizzate

- Python
- PyTorch / Torchvision
- Matplotlib
- Google Colab

---

## 📁 Struttura repository (consigliata)

- `dreamscapes_style_transfer.ipynb` → notebook principale
- `outputs/` → immagini generate (finali)
- `assets/` → (opzionale) immagini di esempio a bassa risoluzione
- `README.md`

> Nota: se le immagini originali sono soggette a licenza o molto pesanti, è consigliabile non caricarle nella repo. In alternativa, inserire link e crediti.

---

## ✅ Risultato

L’output finale mantiene la struttura riconoscibile dell’immagine di contenuto, ma introduce una trasformazione cromatica e testurale che richiama una dimensione **surreale e onirica**.

---

## 🔮 Sviluppi futuri

- Confronto con modelli **text-to-image** (es. Stable Diffusion)
- Esperimenti con diversi layer/pesi (morbido vs intenso)
- Versione “serie” con più output e confronto sistematico

---

