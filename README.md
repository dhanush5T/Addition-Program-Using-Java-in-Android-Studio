# Addition Program Using Java in Android Studio

## Project Description
This project is a simple Android application developed using Java in Android Studio. It performs addition of two numbers and displays the result.

## Objective
To develop an Android application that adds two numbers entered by the user.

## Software Requirements
- Android Studio
- Java Programming Language
- XML

## Working Procedure
1. Open Android Studio.
2. Create a new Android project.
3. Design the user interface using XML.
4. Add two EditText fields to enter numbers.
5. Add one Button to perform addition.
6. Write Java code to add the two numbers.
7. Display the result using a TextView.
8. Run the application.

## Java Program

```java
package com.example.addition;

import android.os.Bundle;
import android.widget.*;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    EditText num1, num2;
    Button add;
    TextView result;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        num1 = findViewById(R.id.num1);
        num2 = findViewById(R.id.num2);
        add = findViewById(R.id.add);
        result = findViewById(R.id.result);

        add.setOnClickListener(v -> {
            int a = Integer.parseInt(num1.getText().toString());
            int b = Integer.parseInt(num2.getText().toString());
            result.setText("Sum = " + (a + b));
        });
    }
}
```

## Output
Enter two numbers in the application and click the ADD button. The application displays their sum.

Example:

First Number = 10

Second Number = 20

Result = 30

## Conclusion
Thus, the addition of two numbers was successfully implemented using Java in Android Studio.
