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
* Problem 1: Unknown Words (OOV – Out of Vocabulary)

Imagine model sees a new word:
"unhappiness"
Word tokenizer → ❌ doesn't know this word
So it marks it as(unknown)
Meaning is lost 😞

* Problem 2: Very Large Vocabulary
Every word must be stored separately(as every words have different ending but still save as unique vocabulary as all have different latter in it)
Example:
play
playing
played
player
📌 Result:
Huge memory required
Slower model

* Problem 3: No Understanding of Word Structure

Word tokenizer treats:
play ≠ playing ≠ played
But actually they are related!


# 3. How Subword Tokenization Solves These Problems
**Models like BERT and GPT use subword tokenization.**
* Advantage 1: Handles Unknown Words
> unhappiness → un + happy + ness

Even if full word is new:
1. "happy" is known
2. "un" = not
3. "ness" = state
👉 Model understands meaning correctly

* Advantage 2: Smaller Vocabulary
Instead of storing:
__play, playing, played, player__
Store:
- *play + ing + ed + er*




