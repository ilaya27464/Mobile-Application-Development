# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:


## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by: ILayaraja M
Registeration Number : 212221040057
*/
```
## activty_main.xml:
```
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"

    xmlns:app="http://schemas.android.com/apk/res-auto"

    xmlns:tools="http://schemas.android.com/tools"

    android:layout_width="match_parent"

    android:layout_height="match_parent"

    tools:context=".MainActivity">

    <Button
        android:id="@+id/colorButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:text="Change Color"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/fontButton"
        app:layout_constraintVertical_bias="0.082" />

    <Button
        android:id="@+id/fontButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/colorButton"
        android:layout_centerHorizontal="true"
        android:layout_marginStart="120dp"
        android:layout_marginTop="120dp"
        android:text="Change Font"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_below="@id/fontButton"
        android:layout_centerHorizontal="true"
        android:text="Hello World!"
        android:textSize="40sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.435"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.325" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java:
```
package com.example.colorfont;

import androidx.appcompat.app.AppCompatActivity;

import android.graphics.Color;

import android.graphics.Typeface;

import android.os.Bundle;

import android.view.View;

import android.widget.Button;

import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    private Button colorButton;

    private Button fontButton;

    private TextView textView;

    @Override

    protected void onCreate(Bundle savedInstanceState) {

        super.onCreate(savedInstanceState);

        setContentView(R.layout.activity_main);

        colorButton = findViewById(R.id.colorButton);

        fontButton = findViewById(R.id.fontButton);

        textView = findViewById(R.id.textView);

        colorButton.setOnClickListener(new View.OnClickListener() {

            @Override

            public void onClick(View v) {

                changeTextColor();

            } });

        fontButton.setOnClickListener(new View.OnClickListener() {

            @Override

            public void onClick(View v) {

                changeFont();

            }
        });
    }
    private void changeTextColor() {

        int randomColor = Color.rgb(

                (int) (Math.random() * 256),

                (int) (Math.random() * 256),

                (int) (Math.random() * 256)
        );
        textView.setTextColor(randomColor);
    }
    private void changeFont() {

        Typeface[] fontStyles = new Typeface[]{

                Typeface.DEFAULT,

                Typeface.DEFAULT_BOLD,

                Typeface.MONOSPACE,

                Typeface.SANS_SERIF,

                Typeface.SERIF

        };

        int randomIndex = (int) (Math.random() * fontStyles.length);
        Typeface selectedFont = fontStyles[randomIndex];
        textView.setTypeface(selectedFont);}
}
```


## OUTPUT
![Screenshot (320)](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/6b168306-e229-4b4f-b136-15d2f5a1b8b2)
![Screenshot (322)](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/b9986075-b5d6-40e3-a933-880986fba9b3)



## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


