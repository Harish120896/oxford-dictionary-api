# oxford-dictionary-api
A node module for easy access of oxford-dictionary api

### Usage
```javascript
const Dictionary = require('oxford-dictionary-api');

const app_id = 'your oxford-account app id';
const app_key = 'your oxford-account app key';
const dict = new Dictionary(app_id, app_key);
dict.find('ace', (error, data) => { if (error) return console.log(error); console.log(data); });
```

Response is a JSON object from which you can access the required details such as definition, type, audio files, example statements:

```json
  {
  "metadata": {
    "provider": "Oxford University Press"
  },
  "results": [
    {
      "id": "ace",
      "language": "en",
      "lexicalEntries": [
        {
          "entries": [
            {
              "grammaticalFeatures": [
                {
                  "text": "Positive",
                  "type": "Degree"
                }
              ],
              "homographNumber": "001",
              "senses": [
                {
                  "definitions": [
                    "very good:"
                  ],
                  "examples": [
                    {
                      "text": "Ace! You've done it!"
                    },
                    {
                      "text": "an ace swimmer"
                    }
                  ],
                  "id": "m_en_gb0004640.006",
                  "registers": [
                    "informal"
                  ]
                }
              ]
            }
          ],
          "language": "en",
          "lexicalCategory": "Adjective",
          "pronunciations": [
            {
              "audioFile": "http://audio.oxforddictionaries.com/en/mp3/ace_gb_1.mp3",
              "dialects": [
                "British English"
              ],
              "phoneticNotation": "IPA",
              "phoneticSpelling": "eɪs"
            }
          ],
          "text": "ace"
        },
        {
          "entries": [
            {
              "etymologies": [
                "Middle English (denoting the ‘one’ on dice): via Old French from Latin as unity, a unit"
              ],
              "grammaticalFeatures": [
                {
                  "text": "Singular",
                  "type": "Number"
                }
              ],
              "homographNumber": "000",
              "senses": [
                {
                  "definitions": [
                    "a playing card with a single spot on it, ranked as the highest card in its suit in most card games:"
                  ],
                  "domains": [
                    "Cards"
                  ],
                  "examples": [
                    {
                      "registers": [
                        "figurative"
                      ],
                      "text": "life had started dealing him aces again"
                    },
                    {
                      "text": "the ace of diamonds"
                    }
                  ],
                  "id": "m_en_gb0004640.001"
                },
                {
                  "definitions": [
                    "a person who excels at a particular sport or other activity:"
                  ],
                  "domains": [
                    "Sport"
                  ],
                  "examples": [
                    {
                      "text": "a motorcycle ace"
                    }
                  ],
                  "id": "m_en_gb0004640.002",
                  "registers": [
                    "informal"
                  ],
                  "subsenses": [
                    {
                      "definitions": [
                        "a pilot who has shot down many enemy aircraft:"
                      ],
                      "domains": [
                        "Air Force"
                      ],
                      "examples": [
                        {
                          "text": "a Battle of Britain ace"
                        }
                      ],
                      "id": "m_en_gb0004640.003",
                      "registers": [
                        "informal"
                      ]
                    }
                  ]
                },
                {
                  "definitions": [
                    "(in tennis and similar games) a service that an opponent is unable to return and thus wins a point:"
                  ],
                  "domains": [
                    "Tennis"
                  ],
                  "examples": [
                    {
                      "text": "Nadal banged down eight aces in the set"
                    }
                  ],
                  "id": "m_en_gb0004640.004",
                  "subsenses": [
                    {
                      "definitions": [
                        "a hole in one:"
                      ],
                      "domains": [
                        "Golf"
                      ],
                      "examples": [
                        {
                          "text": "his hole in one at the 15th was Senior's second ace as a professional"
                        }
                      ],
                      "id": "m_en_gb0004640.005",
                      "registers": [
                        "informal"
                      ]
                    }
                  ]
                }
              ]
            }
          ],
          "language": "en",
          "lexicalCategory": "Noun",
          "pronunciations": [
            {
              "audioFile": "http://audio.oxforddictionaries.com/en/mp3/ace_gb_1.mp3",
              "dialects": [
                "British English"
              ],
              "phoneticNotation": "IPA",
              "phoneticSpelling": "eɪs"
            }
          ],
          "text": "ace"
        },
        {
          "entries": [
            {
              "grammaticalFeatures": [
                {
                  "text": "Transitive",
                  "type": "Subcategorization"
                },
                {
                  "text": "Present",
                  "type": "Tense"
                }
              ],
              "homographNumber": "002",
              "senses": [
                {
                  "definitions": [
                    "(in tennis and similar games) serve an ace against (an opponent):"
                  ],
                  "domains": [
                    "Tennis"
                  ],
                  "examples": [
                    {
                      "text": "he can ace opponents with serves of no more than 62 mph"
                    }
                  ],
                  "id": "m_en_gb0004640.007",
                  "registers": [
                    "informal"
                  ],
                  "subsenses": [
                    {
                      "definitions": [
                        "score an ace on (a hole) or with (a shot):"
                      ],
                      "domains": [
                        "Golf"
                      ],
                      "examples": [
                        {
                          "text": "there was a prize for the first player to ace the hole"
                        }
                      ],
                      "id": "m_en_gb0004640.008"
                    }
                  ]
                },
                {
                  "definitions": [
                    "achieve high marks in (a test or exam):"
                  ],
                  "examples": [
                    {
                      "text": "I aced my grammar test"
                    }
                  ],
                  "id": "m_en_gb0004640.009",
                  "regions": [
                    "North American"
                  ],
                  "registers": [
                    "informal"
                  ],
                  "subsenses": [
                    {
                      "definitions": [
                        "outdo someone in a competitive situation:"
                      ],
                      "examples": [
                        {
                          "text": "the magazine won an award, acing out its rivals"
                        }
                      ],
                      "id": "m_en_gb0004640.010",
                      "regions": [
                        "North American"
                      ]
                    }
                  ]
                }
              ]
            }
          ],
          "language": "en",
          "lexicalCategory": "Verb",
          "pronunciations": [
            {
              "audioFile": "http://audio.oxforddictionaries.com/en/mp3/ace_gb_1.mp3",
              "dialects": [
                "British English"
              ],
              "phoneticNotation": "IPA",
              "phoneticSpelling": "eɪs"
            }
          ],
          "text": "ace"
        }
      ],
      "type": "headword",
      "word": "ace"
    }
  ]
}
```
