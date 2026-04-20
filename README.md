# SubWord Tokenization
✅ Word Tokenization
Splits sentence into full words.
"I am playing cricket"
→ I | am | playing | cricket

✅ Subword Tokenization
Splits words into smaller meaningful parts
	playing → play + ing
	cricket → crick + et

---
# 2. Problems with Word Tokenization
❌ Problem 1: Unknown Words (OOV – Out of Vocabulary)

Imagine model sees a new word:
"unhappiness"
Word tokenizer → ❌ doesn't know this word
So it marks it as(unknown)
Meaning is lost 😞

* Problem 2: Very Large Vocabulary
Every word must be stored separately
Example:
play
playing
played
player

👉 All stored as different words

📌 Result:

Huge memory required
Slower model

