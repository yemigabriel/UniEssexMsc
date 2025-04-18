## Parse Tree Activity

### Phrase 1: The government raised interest rates.

```
(S
  (NP (DT The) (NN government))
  (VP (VBD raised)
      (NP (NN interest) (NNS rates)))
  (. .))
```

### Phrase 2: The internet gives everyone a voice.

```
(S
  (NP (DT The) (NN internet))
  (VP (VBZ gives)
      (NP (NN everyone))
      (NP (DT a) (NN voice)))
  (. .))
```

### Phrase 3: The man saw the dog with the telescope.

*Note: This sentence is syntactically ambiguous. Two possible parse trees are given below.*

**Interpretation A: The man used the telescope to see the dog.**
```
(S
  (NP (DT The) (NN man))
  (VP (VBD saw)
      (NP (NP (DT the) (NN dog))
          (PP (IN with)
              (NP (DT the) (NN telescope)))))
  (. .))
```

**Interpretation B: The dog has the telescope.**
```
(S
  (NP (DT The) (NN man))
  (VP (VBD saw)
      (NP (DT the) (NN dog)
          (PP (IN with)
              (NP (DT the) (NN telescope)))))
  (. .))
```

---

### Explanation

This activity demonstrates the structure of natural language using constituency-based parse trees. Each sentence is broken down into nested constituents, where:
- **NP** = Noun Phrase
- **VP** = Verb Phrase
- **PP** = Prepositional Phrase
- **DT** = Determiner
- **NN/NNS** = Noun (singular/plural)
- **VBD/VBZ** = Verb (past tense/present tense)
- **.** = Sentence-ending punctuation

Understanding constituency parsing is essential for tasks such as syntactic analysis, machine translation, and information extraction. The third sentence illustrates syntactic ambiguity, showing how different structures can lead to different meanings, a key consideration in intelligent systems dealing with natural language understanding.

