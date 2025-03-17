### **🔹 Simple Sentiment Analysis Example (IMDB Dataset)**  

#### **1️⃣ Overview**
- Uses **Keras** (a deep learning library) for **sentiment analysis**.  
- Analyzes **IMDB movie reviews** to classify them as **positive or negative**.  
- Uses a **Perceptron model** (basic neural network).  

---

#### **2️⃣ Getting Started**  
**Steps to set up and run the project:**  
```bash
git clone https://github.com/philipperemy/Sentiment-Analysis-NLP.git
cd Sentiment-Analysis-NLP
chmod +x init.sh
./init.sh
python main_perceptron.py
```
- Downloads and extracts the **IMDB Sentiment Database** from Stanford.  
- Uses a **word list** of **6,800 positive/negative words** from Illinois University.  

---

#### **3️⃣ Execution Output (Example)**  
- Loads **positive and negative words**.  
- Processes **5,000 positive & 5,000 negative reviews**.  
- Starts **training the neural network** with **TensorFlow** backend.  
- Runs for **200 epochs** (iterations).  

Example output:  
```
=> loaded 2006 positive words
=> loaded 4783 negative words
=> processed 5000 aclImdb/train/neg files.
=> processed 5000 aclImdb/train/pos files.
Epoch 1/200
6666/6666 [==============================] - 22s - loss: 0.2177
```

---

#### **4️⃣ Accuracy Results**  
- **Training accuracy:** **80.3%**  
- **Validation accuracy:** **73.3%**  
*(Can be improved with more training and tuning.)*  

---

#### **5️⃣ Visualizing the Model with TensorBoard**  
- Ensure **Keras backend** is **TensorFlow** (`cat ~/.keras/keras.json`).  
- Run TensorBoard to view training progress:  
```bash
tensorboard --logdir=deep_learning/runs/1455792487
```

---

✅ **Conclusion:** This project uses deep learning for **sentiment analysis** on IMDB reviews, achieving **~80% accuracy**. 
