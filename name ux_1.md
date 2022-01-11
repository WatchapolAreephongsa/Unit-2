```py
def UX_terms(word):
    terms = ["usability","usefulness","desirability"]
    definition = ["a quality attribute that assesses how easy user interfaces are to use." ,"the quality of having utility and especially practical worth or applicability.", "the quality of being sexually attractive"]
    for i in range (3):
        if terms[i] == word:
            result = f"{word} is {definition[i]}"
    return result
print(UX_terms("desirability"))
```
