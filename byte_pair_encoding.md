
# Byte Pair Encoding
Byte Pair Encoding (BPE) is a subword tokenization technique used in NLP to break words into smaller parts based on frequency.

Why do we use BPE?<br>
Because: <br>
Words can be too many (huge vocabulary) <br>
New words appear often <br>
👉 BPE helps by: <br>
Reducing vocabulary size <br>
Handling unknown words <br>
Creating meaningful subwords <br>

How BPE Works (Step-by-Step)<br>
🔸 Step 1: Start with characters <br>
Suppose we have words: <br>
low, lower, lowest <br>
Break into characters: <br>
lo w <br>
lo w e r <br>
lo w e s t <br>
🔸 Step 4: Repeat merging <br>
Next frequent pair: <br>
lo + w → "low" <br>
Now: <br>
low <br>
low e r <br>
low e s t <br>
🔸 Step 5: Continue <br>

Next merges: <br>

e + r → er   <br>
e + s → es   <br>
es + t → est <br>

Final tokens: <br>

low, er, est <br>
🔹 Final Result <br>

👉 Instead of storing full words: <br>

**low, lower, lowest** <br>

👉 BPE stores: <br>

**low, er, est**
