# enum

```
enum Emotion {
    Happy,
    Sad,
    Excited,
}

var howIFeel = Emotion.Sad;

if howIFeel == Emotion.Sad {
    stdout.write_line("I am sad. I will eat an ice cream cone.");
    howIFeel = Emotion.Excited;
    eatTastyIceCream();
    howIFeel = Emotion.Happy;
}

if howIFeel == Emotion.Happy {
    stdout.write_line("I feel great!");
}

```
