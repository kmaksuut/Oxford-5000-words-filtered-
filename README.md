# Oxford‑5000 Words (Filtered Edition)

Original project: [tyypgzl / Oxford‑5000‑words](https://github.com/tyypgzl/Oxford-5000-words) ([GitHub](https://github.com/tyypgzl/Oxford-5000-words))

This repository contains a filtered version of the *Oxford 5000 Word List* tailored to specific requirements.  
It references the original dataset while applying modifications (removing certain fields).

---

## 🧾 Removes

- Remove audio links
- Remove "uk" phonetic

---

## Data Modifications / Changes

In the original `full-word.json`, each entry had a structure like this:

```json
    {
        "id": 0,
        "value": {
            "word": "a",
            "href": "https://www.oxfordlearnersdictionaries.com/definition/english/a_1",
            "type": "indefinite article",
            "level": "A1",
            "us": {
                "mp3": "https://www.oxfordlearnersdictionaries.com/media/english/us_pron/a/a__/a__us/a__us_2_rr.mp3",
                "ogg": "https://www.oxfordlearnersdictionaries.com/media/english/us_pron_ogg/a/a__/a__us/a__us_2_rr.ogg"
            },
            "uk": {
                "mp3": "https://www.oxfordlearnersdictionaries.com/media/english/uk_pron/a/a__/a__gb/a__gb_2.mp3",
                "ogg": "https://www.oxfordlearnersdictionaries.com/media/english/uk_pron_ogg/a/a__/a__gb/a__gb_2.ogg"
            },
            "phonetics": {
                "us": "/eɪ/",
                "uk": "/eɪ/"
            },
            "examples": [
                "a man/horse/unit",
                "an aunt/egg/hour/X-ray",
                "I can only carry two at a time.",
                "There's a visitor for you.",
                "She's a friend of my father's (= one of my father's friends)."
            ]
        }
    }
```

Filtered data like this :

```json
  {
    "id": 0,
    "value": {
      "word": "a",
      "href": "https://www.oxfordlearnersdictionaries.com/definition/english/a_1",
      "type": "indefinite article",
      "level": "A1",
      "examples": [
        "a man/horse/unit",
        "an aunt/egg/hour/X-ray",
        "I can only carry two at a time.",
        "There's a visitor for you.",
        "She's a friend of my father's (= one of my father's friends)."
      ],
      "phonetics": {
        "us": "/eɪ/"
      }
    }
  },
```
<hr>

### Turkish-English Translate

**EN** : The translations were generated automatically using the ``Google Translate API`` and ``Node.js``.

**TR** : Çeviri ``Google Translate API`` ile yapılmıştır ve ``Node.js`` ile otomatik olarak oluşturulmuştur.

```json
{
    "id": 436,
    "value": {
      "word": {
        "en": "ball",
        "tr": "top"
      },
      "href": "https://www.oxfordlearnersdictionaries.com/definition/english/ball_1",
      "type": "noun",
      "level": "A1",
      "examples": [
        "a golf/tennis/bowling/soccer ball ",
        "to hit/throw/kick/catch a ball",
        "He kicked the ball into the net.",
        "Bounce the ball and try and hit it over the net.",
        "The kids were playing with a bat and ball in the park.",
        "The ball bounced off down the road."
      ],
      "phonetics": {
        "us": "/bɔːl/"
      }
    }
  }
```
