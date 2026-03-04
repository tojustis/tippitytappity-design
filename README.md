# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

---
title: TippityTappity
---
classDiagram
  Skills <|-- Typing
  class Skills{
        + rank: int
        - accuracy: float
        - speed: double
        - calcAcc()
        - calcSpeed()
  }
  class Typing{
        - time: double
        - keystroke: char
        - word: vector~string~
        - randomWord(worldList)
        - matchKeyToWord(words,keystroke)
        - measureTime(time)
        - getWPM()

  }



