# tippitytappity-design

tippitytappity is a program to practice typing


## Data model

```mermaid
classDiagram
  Test <|-- User
  Phrase <|-- Test
  class User{
        + ID: string
        + username: string
        + password: string
        - login(user: string, pass: string) boolean
        - get_email() string
  }
  class Test{
        + ID: string
        + started: date
        + finished: date
        + wpm: float
        + accuracy: float
  }
  class Phrase{
        + ID: string
        + content: string
  }
```
