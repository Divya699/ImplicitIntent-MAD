# Ex.No:3a Develop program to create a text field and a button “Navigate”. When you enter “www.gmail.com” and press navigate button it should open google page using Implicit Intents.


## AIM:

To create a navigate button using Implicit Intent to display the gmail page using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

1. Start the project: Create a new Android project in Android Studio.
2. Design the UI: In activity_main.xml, add an EditText (to accept the URL input) and a Button (to trigger the navigation).
3. Initialize components: In MainActivity.java, map the EditText and Button variables to their respective XML IDs using findViewById().
4. Set click listener: Attach an OnClickListener to the button to listen for user click events.
5. Get input: Inside the onClick method, extract the text entered in the EditText and convert it to a string.
6. Create implicit intent: Instantiate an Intent with the action Intent.ACTION_VIEW and pass the parsed URL string using Uri.parse().
7. Start activity: Call startActivity(intent) to trigger the OS to open the webpage in an available web browser.
8. Execution: Run and test the application.



## PROGRAM:
### MainActivity.java
```
package com.example.lifecycleactivity;

import android.os.Bundle;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG)
        toast.show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onPause() {
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onStop() {
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG)
        toast.show();
    }

}

 
```
### activity_main_xml

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="199dp"
        android:layout_height="25dp"
        android:autoSizeTextType="none"
        android:fontFamily="sans-serif-black"
        android:text="Hello Everyone"
        android:textAlignment="center"
        android:textColor="#1131D9"
        android:textSize="20sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.473" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="sans-serif-black"
        android:text="Welcome to Life Cycle Activity"
        android:textAlignment="center"
        android:textColor="#CE1313"
        android:textSize="20sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.321" />

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Start your Activity"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        tools:layout_editor_absoluteY="429dp" />

    <ImageView
        android:id="@+id/imageView2"
        android:layout_width="124dp"
        android:layout_height="80dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.498"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button2"
        app:layout_constraintVertical_bias="0.132"
        app:srcCompat="@android:drawable/ic_media_play" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT

<img width="1873" height="1006" alt="Screenshot 2026-10-22 113618" src="https://github.com/user-attachments/assets/9d15fe22-9f85-41b3-ab0e-ee4e81e7a246" />



## RESULT
Thus a Simple Android Application create a navigate button using Implicit Intent to display the gmail page using Android Studio is developed and executed successfully.


