# Quiz app

![quiz-images](readme/app-images.png)

Quiz app made for web programming Made with android studio

# Acquired knowledge
* Work with more than one **activity**
* The use of **RadioGroup** and **RadioButtom**
* Use the **Constraint layout**
* Send **data** from one **activity** to another
* Using `MediaPlayer` to play a sound in the app

# 
quiz questions

Questions were added by the `Question` class

`Question` class

```java
public class Question {

    private String question;
    private List<String> answers = new ArrayList<>();
    private String rightAnswer;

    public Question(String question,String rightAnswer, String ... answers ) {
        this.question = question;
        this.rightAnswer = rightAnswer;s
        this.answers.add(answers[0]);
        this.answers.add(answers[1]);
        this.answers.add(answers[2]);
        this.answers.add(answers[3]);
    }


    public String getQuestion() {
        return question;
    }

    public List<String> getAnswers() {
        return answers;
    }

    public String getRightAnswer() {
        return rightAnswer;
    }
}
```



Example of using the `Question` class:

```java
questions = new ArrayList<Question>(){
            {

               add(new Question("Under which of the following Android is licensed?", "D", "Sourceforge", "OSS","None of the above", "Apache/MIT"));
                add(new Question("For which of the following Android is mainly developed?", "A", "Mobile devices", "Laptops","Desktops", "Servers"));
                add(new Question("Which of the following is the first mobile phone released that ran the Android OS?", "D", "HTC Hero", "Google gPhone","None of the above", "T - Mobile G1"));
                add(new Question("Which of the following virtual machine is used by the Android operating system?", "B", "JVM", "Dalvik virtual machine", "Simple virtual machine", "None of the above"));
                add(new Question(" Android is based on which of the following language?", "A", "Java", "C++", "C", "None of the above"));
                add(new Question("APK stands for -", "D", "None of the above", "Android Phone Kit", "Android Page Kit", "Android Package Kit"));
                add(new Question("Which of the following converts Java byte code into Dalvik byte code?", "C", "Dalvik converter", "Mobile interpretive compiler (MIC)", "Dex compiler", "None of the above"));
                add(new Question("How can we stop the services in android?", "B", "By using the finish() method", "By using the stopSelf() and stopService() method", "By using system.exit() method", "None of the above"));
                add(new Question("What is an activity in android?", "B", "android class", "A single screen in an application with supporting java code", "android package", "None of the above"));
                add(new Question("How can we kill an activity in android?", "D", "Using finish() method", "Using finishActivity(int requestCode)", "Neither (a) nor (b)", "Both (a) and (b)"));
            }
        };
```

___
<h4 align="center">
    Feito com 💜 by  Vitor Carmo
</h4>
