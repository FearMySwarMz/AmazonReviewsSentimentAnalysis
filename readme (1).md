# Amazon Review Sentiment Analysis με Word2Vec, GloVe & BERT

## Περιγραφή
Το project αυτό υλοποιεί ανάλυση συναισθήματος (sentiment analysis) σε κριτικές προϊόντων της Amazon χρησιμοποιώντας **Word2Vec**, **GloVe** και **BERT embeddings** (freezed & fine-tuned), σε συνδυασμό με αλγορίθμους μηχανικής μάθησης και deep learning. Περιλαμβάνει προεπεξεργασία κειμένου, εκπαίδευση μοντέλου Word2Vec, μετατροπή κριτικών σε διανύσματα χαρακτηριστικών και αξιολόγηση ταξινομητή.

## Περιεχόμενα Repository
- `AmazonReviewSentimentAnalysis.ipynb`: Jupyter Notebook με όλη τη ροή του project
  - Καθαρισμός και προεπεξεργασία κειμένου (regex, tokenization)
  - Εκπαίδευση Word2Vec μοντέλου
  - Δημιουργία embeddings για κάθε κριτική
  - Εκπαίδευση ταξινομητή συναισθήματος
  - Αξιολόγηση απόδοσης με κατάλληλα metrics

## Τεχνολογίες & Βιβλιοθήκες
- Python
- Jupyter Notebook
- NumPy
- pandas
- gensim (Word2Vec)
- pre-trained GloVe embeddings
- Hugging Face Transformers (BERT)
- scikit-learn

## Ροή Εργασίας
1. **Προεπεξεργασία Κειμένου**  
   Καθαρισμός κριτικών από θόρυβο (σύμβολα, αριθμούς, timestamps κ.λπ.) και μετατροπή σε tokens.

2. **Embeddings Κειμένου**  
   - Εκπαίδευση Word2Vec μοντέλου
   - Χρήση προεκπαιδευμένων GloVe embeddings
   - BERT embeddings σε *freezed* mode
   - BERT *fine-tuned* για sentiment analysis

3. **Αναπαράσταση Κριτικών**  
   Μετατροπή κάθε κριτικής σε διάνυσμα χαρακτηριστικών (μέσος όρος embeddings ή CLS token για BERT).

4. **Ταξινόμηση Συναισθήματος**    
   Υπολογισμός ενός ενιαίου διανύσματος για κάθε κριτική (π.χ. μέσω μέσου όρου των word vectors).

4. **Ταξινόμηση Συναισθήματος**  
   Εκπαίδευση μοντέλου μηχανικής μάθησης για πρόβλεψη θετικού/αρνητικού συναισθήματος.

5. **Αξιολόγηση & Σύγκριση Μοντέλων**  
   Μέτρηση απόδοσης με metrics όπως accuracy, precision, recall και F1-score.

## Πώς να Τρέξετε το Project
1. Κάντε clone το repository:
   ```bash
   git clone https://github.com/username/repository-name.git
   ```
2. Εγκαταστήστε τις απαιτούμενες βιβλιοθήκες:
   ```bash
   pip install -r requirements.txt
   ```
   *(ή εγκαταστήστε τες χειροκίνητα αν δεν υπάρχει requirements.txt)*
3. Ανοίξτε το notebook:
   ```bash
   jupyter notebook AmazonReviewSentimentAnalysis.ipynb
   ```

## Στόχος Project
Στόχος είναι η σύγκριση διαφορετικών τεχνικών αναπαράστασης κειμένου (**Word2Vec, GloVe, BERT freezed, BERT fine-tuned**) ως προς την απόδοσή τους στο sentiment analysis πραγματικών δεδομένων.

Στόχος είναι η κατανόηση και εφαρμογή τεχνικών **NLP** και **distributed word representations** (Word2Vec) για την ανάλυση συναισθήματος πραγματικών δεδομένων κριτικών.

## Μελλοντικές Βελτιώσεις
- Χρήση πιο προχωρημένων embeddings (GloVe, FastText, BERT)
- Πειραματισμός με διαφορετικούς ταξινομητές
- Βελτιστοποίηση υπερπαραμέτρων

---
*Educational / Academic Project*

