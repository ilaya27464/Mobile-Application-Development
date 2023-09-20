# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: ILAYARAJA M
Registeration Number : 212221040057
*/
```
# activity_main.xml:
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout
    xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    style="TIM"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World\nThis is Ashmi."
        android:textSize="30dp"
        android:textAppearance="@style/TextAppearance.AppCompat.Large"
        android:textColorHighlight="#FFFFFF"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.455"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_baias="0.407" />

</androidx.constraintlayout.widget.ConstraintLayout>
```
# MainActivity.java:
```
package com.example.lifecyclehello;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;
public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast.makeText(this, "onCreate Called", Toast.LENGTH_SHORT).show();
    }

    @Override
    protected void onRestart(){
        Toast.makeText(this, "onRestart Called", Toast.LENGTH_SHORT).show();
        super.onRestart();
    }
    @Override
    protected void onStart(){
        Toast.makeText(this, "onStart Called", Toast.LENGTH_SHORT).show();

        super.onStart();
    }
    @Override
    protected void onResume(){
        Toast.makeText(this, "onResume Called", Toast.LENGTH_SHORT).show();

        super.onResume();
    }
    @Override
    protected void onPause(){
        Toast.makeText(this, "onPause Called", Toast.LENGTH_SHORT).show();

        super.onPause();
    }
    @Override
    protected void onStop(){
        Toast.makeText(this, "onStop Called", Toast.LENGTH_SHORT).show();

        super.onStop();
    }
    @Override
    protected void onDestroy(){
        Toast.makeText(this, "onDestroy Called", Toast.LENGTH_SHORT).show();

        super.onDestroy();
    }
}
```

## OUTPUT


![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/1534d00b-62a3-4bf2-9549-dbed06bfbe93)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/46281ee3-45a2-4864-b3af-c8fdea960a32)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/8cabc0f6-f026-4e82-9b6d-72a38b2330b9)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/4d271140-9bb9-47c9-a20f-70f8a3c08a8e)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/ff457074-e653-4ffe-b161-56599abf5a22)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/115fd65e-6263-4435-9ad8-6c91b234bd67)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/127576283/c77855d3-e1d4-43a8-af1d-468fbd650fb0)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
