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
Developed by: ASHMI S
Registeration Number : 212221040021
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


![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/9a797a2a-1d91-44c3-a47a-0c2124b29f1d)
![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/72f80164-cbf4-4707-9175-3672d715e902)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/4b56a759-ab4d-4614-82ed-377a3ca730fb)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/c02f3957-4e3d-49c8-954b-b8b38b318ae7)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/8c2e917f-2ee8-4173-9c04-cf5d29eb44c3)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/525b3b25-2453-4ebd-bf87-d3403116fecd)

![image](https://github.com/suryacse05/Mobile-Application-Development/assets/103128410/1d40ed54-57d3-45d5-a19b-98ab6246f95a)



## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
