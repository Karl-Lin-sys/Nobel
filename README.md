# Nobel: a little box of words

*A read-aloud explanation in Canadian English. A grown-up can read it with you.*

## Open the box

Imagine a box of little cards.
There are **47 cards** inside.
Each card has some English words.
Each card also has a time, like **4:21**.
The time helps us find that part of the chat.

The words come from one reported online chat.
People talk about Nobel Prizes and science.
They get excited. They say thank you. They make jokes, too!

This computer project keeps those words tidy.

## Make little piles

Imagine using a different colour for each pile.

- **14 cards** have everyday chat.
- **13 cards** talk about chemistry: what things are made of and how they change.
- **2 cards** talk about medicine: learning about our bodies and helping us stay well.
- **18 cards** talk about physics: how things in our world work.

Those are the labels in this box.
A label helps us sort. It does not tell us that every sentence is right.

## Keep the old words, too

Someone tidied the English on **eight cards**.
The old words are still there.
You can look at the old words and the new words together.

Two cards say the same thing at different times.
We keep both cards, because both times matter.

## Find the missing friend

A translation says the same idea in another language.
Think of two cards holding hands:
one has Japanese words, and one has English words.

Here, we have the English cards.
The Japanese cards are missing.
We leave their spaces empty.
We do not guess what they said.

A person needs to find the real Japanese words and check the pairs.
**No pairs are ready yet.**

## Give the computer a fair turn

Imagine practising one song again and again.
You might sing it very well!
But can you sing a new song?

A computer needs a fresh test, too.
These cards come from just one reported chat.
We need other chats for a fair test.
We also need to check every pile, even the tiny one.

## What can this box do?

The program puts the cards in order.
It checks their time labels.
It finds repeated words.
It shows what still needs a person to check.

It has not taught a computer to translate yet.
It cannot tell us that the prize and science stories are all true.
Those stories still need checking.

**For now, we have a tidy box of words, with room to learn more.**

---

## For grown-ups

This explanation describes the supplied `Nobel-Corpus-Package.zip`. The cards are an analogy for its text records; no physical or coloured cards are included. The topic definitions above are broad child-friendly descriptions, not verification of the scientific statements in the submitted translations.

The package contains 47 timestamped English records, 46 distinct normalised original texts, eight editorial changes, one reported stream, and zero approved Japanese–English pairs. The original Japanese, video URL, and stream date are missing. No model has been trained or evaluated.

All 20 original package files are preserved: the supplied README is saved as [ORIGINAL_README.md](ORIGINAL_README.md), and this page is the new child-friendly entry point. The supplied research, software-version, and verification documents remain records from the attachment; publishing them does not independently confirm their claims. See [this upload's checks](docs/publication_checks.md) for checks actually rerun here.

| Open this | What you will find |
| --- | --- |
| [Original English](data/raw/translations.txt) | The submitted words and times. |
| [Organised cards](data/processed/corpus.jsonl) | One computer-readable record per line, called JSONL. |
| [Data card](data/DATA_CARD.md) | Counts, origins, editing details, and missing information. |
| [Original project guide](ORIGINAL_README.md) | Commands, file links, and the technical explanation. |
| [Original simple explanation](docs/simple_explanation.md) | The explanation already included in the ZIP. |

To check the package with Python 3.10 or later, run these commands from this folder:

```sh
python corpus.py audit data/processed/corpus.jsonl
python -m unittest discover -s tests -v
```

Use `python3` if that is the Python command on your computer. No extra Python packages are needed.
