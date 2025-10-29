# Customer Segmentation Dashboard - Power BI

## Obiettivo
Creare una dashboard interattiva in Power BI per visualizzare i pattern di comportamento dei clienti e identificare segmenti chiave per strategie di marketing mirate.

## Dataset
- **Fonte**: Kaggle - Mall Customers Dataset
- **Righe**: 200 clienti
- **Colonne**: CustomerID, Genre, Age, Annual Income, Spending Score

**Nota**: Dataset sintetico utilizzato per scopi didattici. Alcune anomalie nei dati (es. giovani con redditi molto elevati) confermano la natura simulata del dataset.

---

## Tecnologie
- **Power BI Desktop**
- Data visualization
- Interactive dashboards
- DAX (Data Analysis Expressions) per metriche calcolate

---

## Dashboard Components

### 1. KPI Cards
- **Totale Clienti**: Conteggio totale clienti nel dataset
- **Spending Medio**: Media dello spending score (0-100)
- *Entrambe le card si aggiornano dinamicamente in base ai filtri applicati*

### 2. Scatter Plot - Reddito vs Spending Score
- **Asse X**: Annual Income (k$)
- **Asse Y**: Spending Score (1-100)
- **Colore**: Genere (Male/Female)

**Insight**: Nessuna correlazione lineare evidente tra reddito e propensione alla spesa. I dati mostrano cluster distinti che suggeriscono diversi segmenti di clientela.

### 3. Bar Chart - Spesa Media per Genere
- Confronto diretto tra comportamento di spesa maschile e femminile
- **Risultato**: Le donne mostrano spending score medio superiore

### 4. Column Chart - Distribuzione Clienti per Età
- Visualizzazione della composizione demografica del customer base
- Identifica le fasce d'età più rappresentate

### 5. Interactive Slicers (Filtri)
- **Slicer Età**: Range slider per filtrare per fasce d'età
- **Slicer Genere**: Checkbox per selezionare Male/Female

**Funzionalità**: Tutti i visual si aggiornano in tempo reale quando si applicano filtri

---

## Key Insights

### 1. Gender Differences
- Le clienti donne mostrano propensione alla spesa superiore rispetto agli uomini
- Pattern consistente attraverso diverse fasce di reddito

### 2. Age Patterns
- Clienti più giovani (<30) tendono ad avere spending score più elevati
- Fascia intermedia (30-50) mostra maggiore variabilità
- Clienti senior (50+) mostrano comportamento più conservativo

### 3. Income Paradox
- Non esiste relazione lineare semplice reddito-spesa
- Clienti ad alto reddito (>80k) mostrano sia spending molto alto che molto basso
- Suggerisce segmentazione basata su fattori comportamentali oltre al reddito

### 4. Customer Segments Identificati
- **High spenders, low income**: Giovani con propensione elevata alla spesa
- **High income, moderate spending**: Fascia medio-alta conservativa
- **Balanced**: Reddito e spesa proporzionali (fascia 40-70k)

---

## Business Recommendations

### 1. Targeting per Segmento
- **Giovani (<30)**: Campagne aggressive, prodotti trendy, payment plans
- **Adulti 30-50**: Focus su value proposition, qualità/prezzo
- **Senior high-income**: Prodotti premium, servizi personalizzati

### 2. Gender-Based Marketing
- Maggiore investimento in marketing verso target femminile
- Analisi ulteriore su prodotti preferiti per genere

### 3. Retention Strategy
- Identificare clienti a rischio churn (alto reddito, bassa spesa)
- Programmi loyalty per big spenders

### 4. Product Development
- Linee premium per catturare segmento high-income attualmente non engaged
- Entry-level products per giovani high-spenders con reddito limitato

---

## Interactive Features

La dashboard Power BI permette:
-  Drill-down dinamico** su qualsiasi visualizzazione
-  Cross-filtering**: Click su un grafico filtra automaticamente gli altri
-  Tooltip interattivi** con dettagli aggiuntivi on-hover
-  Export data** da ogni visual per analisi ulteriori
-  Real-time updates** quando si modificano i filtri
