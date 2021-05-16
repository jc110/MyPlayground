# MyPlayground
My First app devlopment project for my android application devlopment class. I am very excited to place in Github.
reate an Android application called My Playground-Done
Using the Android Studio visual designer, add at least 10 different components from the palette to your app. 
Select at least 8 random things that interests you from either Widgets, Text Fields, Containers, Date & Time, etc.. (
Create at least 1 Button
Create at least 1 ImageView, with an image that you added yourself
Position these components wherever you like on the app (using the design tab)-
For each widget, adjust at least 1 property setting to slightly customize the way it looks and/or behaves. 
Run the app on the emulator and get a screenshot of it, using the emulator screenshot feature 

1st page components*********
1.RelativeLayout
2.Textview
3.Button
4.Imageview
5.view
6.Checkbox
7.RadioButton
8.ToggleButton
9.RadioBar
10.ProgressBar
11.TextInputLayout
12.TextInputLayout
13.textView2
*****************************
Code Written to Link to Another Page
package com.example.myplayground;

import android.content.Intent;
import android.view.View;
import android.widget.Button;
import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;

public class MainActivity extends AppCompatActivity {
    //variable button of data type Button
private Button button;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        // Assigning id of button on our design lay out to button variable
        button=findViewById(R.id.button);
        //Setting a click listener to check when button is going to click
        button.setOnClickListener(new View.OnClickListener() {
            //Creating method to open new page when the button is clicked
            @Override
            public void onClick(View v) {
               openActivity2();
            }
        });
    }
    // Opening the second page
    public void openActivity2(){
        Intent intent=new Intent(this,MainActivity2.class);
        startActivity(intent);
    }
}

2nd page components***********
RelativeLayout
ImageView3
