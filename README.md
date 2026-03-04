# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Test <|-- User
  Phrase <|-- Test
  History <|-- User
  class User{
        + ID: string
        + username: string
        + password: string
        + get_progress() vector~vector~int~~
        - login(user: string, pass: string) boolean
        - get_email() string
  }
  class Test{
        + ID: string
        + TestID: string
        + started: date
        + finished: date
        + best_wpm: float
        + best_accuracy: float
  }
  class Phrase{
        + ID: string
        + content: string
  }
  class History{
        +past_wpm: vector~int~
        +past_accuracy: vector~int~
  }

```
