# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Typing <|-- Skills
  Typing <|-- History
  Skills <|-- History
  class Typing{
        - time: double
        - keystroke: char
        - word: string
        - wordList: vector~string~
        - randomWord(worldList)
        - matchKeyToWord(words,keystroke)
        - measureTime(time)
        + getWPM()

  }
  class Skills{
        + rank: int
        - accuracy: float
        - speed: double
        - calcAcc()
        - calcSpeed()
  }

  class History {
        - attemptCount: int
        - attemptTracker: vector~Skill~
        - userName: strings
        - users: vector~string~
        - trackUser(attemptTracker,user)



  }
```


