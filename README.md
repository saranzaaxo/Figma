# Ex09 Event Registration Web Application
## Date:

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```html
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#A34641"
    tools:context=".MainActivity">

    <LinearLayout
        android:id="@+id/teal_container"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:layout_margin="16dp"
        android:background="#2E8B8B"
        android:orientation="vertical"
        android:gravity="center_horizontal"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent">

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:background="@android:color/white"
            android:padding="8dp">

            <ImageView
                android:id="@+id/logo_header"
                android:layout_width="200dp"
                android:layout_height="60dp"
                android:layout_alignParentStart="true"
                android:src="@drawable/saveetha_logo_header"
                android:contentDescription="@string/saveetha_logo_affiliate" />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_alignParentEnd="true"
                android:layout_centerVertical="true"
                android:text="TNEA CODE\n1216"
                android:gravity="center"
                android:textSize="18sp"
                android:textStyle="bold"
                android:textColor="#3F51B5" />
        </RelativeLayout>

        <ImageView
            android:layout_width="250dp"
            android:layout_height="250dp"
            android:layout_marginTop="20dp"
            android:src="@drawable/saveetha_college_logo"
            android:contentDescription="@string/college_logo" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:layout_marginTop="16dp"
            android:text="@string/sports_day_event"
            android:textSize="28sp"
            android:textStyle="bold"
            android:textColor="#FF4081" />

        <Button
            android:id="@+id/btn_register"
            android:layout_width="250dp"
            android:layout_height="60dp"
            android:layout_marginTop="32dp"
            android:text="@string/register"
            android:textSize="24sp"
            android:textStyle="italic"
            android:textColor="@android:color/black"
            android:backgroundTint="#FFEB3B" />

        <Button
            android:id="@+id/btn_login"
            android:layout_width="250dp"
            android:layout_height="60dp"
            android:layout_marginTop="20dp"
            android:text="@string/login"
            android:textSize="24sp"
            android:textStyle="italic"
            android:textColor="@android:color/black"
            android:backgroundTint="#CCCCCC" />

    </LinearLayout>
</androidx.constraintlayout.widget.ConstraintLayout>
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:background="#A34641"
    android:padding="16dp"
    tools:context=".EventSelectionActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        android:background="#FF69B4"
        android:padding="24dp">

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/sports_day_event"
            android:textSize="32sp"
            android:textStyle="bold"
            android:textColor="#3F51B5"
            android:gravity="center_horizontal"
            android:layout_marginBottom="32dp" />

        <RadioGroup
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginBottom="16dp">

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/volley_ball"
                android:textColor="#3F51B5"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/basket_ball"
                android:textColor="#FFFFFF"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/football"
                android:textColor="#FF0000"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/hockey"
                android:textColor="#FFEB3B"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/athlete"
                android:textColor="@android:color/black"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/relay"
                android:textColor="#4CAF50"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

            <RadioButton
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="@string/cricket"
                android:textColor="#00BCD4"
                android:textSize="28sp"
                android:padding="4dp"
                android:buttonTint="#FFFFFF" />

        </RadioGroup>

        <ImageView
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1"
            android:src="@drawable/sports_graphic"
            android:scaleType="centerCrop"
            android:contentDescription="@string/sports_graphic" />

    </LinearLayout>
</LinearLayout>
<?xml version="1.0" encoding="utf-8"?>
<ScrollView xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#A34641"
    tools:context=".RegistrationActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        android:background="@android:color/white"
        android:paddingTop="40dp"
        android:paddingBottom="40dp"
        android:layout_marginTop="32dp"
        android:layout_marginBottom="32dp"
        android:layout_marginStart="16dp"
        android:layout_marginEnd="16dp"
        android:gravity="center_horizontal">

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/event_registration_form"
            android:textSize="30sp"
            android:textStyle="bold|italic"
            android:textColor="@android:color/black"
            android:gravity="center_horizontal"
            android:layout_marginBottom="8dp" />

        <TextView
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="@string/fill_the_details"
            android:textSize="24sp"
            android:textStyle="bold|italic"
            android:textColor="#6A1B9A"
            android:gravity="center_horizontal"
            android:layout_marginBottom="32dp" />

        <EditText
            android:id="@+id/et_full_name"
            android:layout_width="250dp"
            android:layout_height="50dp"
            android:hint="@string/full_name"
            android:textSize="20sp"
            android:textStyle="italic"
            android:textColorHint="@android:color/black"
            android:backgroundTint="#CCCCCC"
            android:paddingStart="10dp"
            android:paddingEnd="10dp"
            android:layout_marginBottom="16dp"
            android:inputType="textPersonName" />

        <EditText
            android:id="@+id/et_gender"
            android:layout_width="250dp"
            android:layout_height="50dp"
            android:hint="@string/gender"
            android:textSize="20sp"
            android:textStyle="italic"
            android:textColorHint="@android:color/black"
            android:backgroundTint="#CCCCCC"
            android:paddingStart="10dp"
            android:paddingEnd="10dp"
            android:layout_marginBottom="16dp"
            android:inputType="textCapWords" />

        <EditText
            android:id="@+id/et_age"
            android:layout_width="250dp"
            android:layout_height="50dp"
            android:hint="@string/age"
            android:textSize="20sp"
            android:textStyle="italic"
            android:textColorHint="@android:color/black"
            android:backgroundTint="#CCCCCC"
            android:paddingStart="10dp"
            android:paddingEnd="10dp"
            android:layout_marginBottom="16dp"
            android:inputType="number" />

        <EditText
            android:id="@+id/et_register_number"
            android:layout_width="250dp"
            android:layout_height="50dp"
            android:hint="@string/register_number"
            android:textSize="20sp"
            android:textStyle="italic"
            android:textColorHint="@android:color/black"
            android:backgroundTint="#CCCCCC"
            android:paddingStart="10dp"
            android:paddingEnd="10dp"
            android:layout_marginBottom="16dp"
            android:inputType="textCapCharacters" />

        <EditText
            android:id="@+id/et_department"
            android:layout_width="250dp"
            android:layout_height="50dp"
            android:hint="@string/department"
            android:textSize="20sp"
            android:textStyle="italic"
            android:textColorHint="@android:color/black"
            android:backgroundTint="#CCCCCC"
            android:paddingStart="10dp"
            android:paddingEnd="10dp"
            android:layout_marginBottom="32dp"
            android:inputType="textCapWords" />

        <Button
            android:id="@+id/btn_form_register"
            android:layout_width="200dp"
            android:layout_height="60dp"
            android:text="@string/register"
            android:textSize="24sp"
            android:textStyle="bold"
            android:textColor="#3F51B5"
            android:backgroundTint="#FF0000" />

    </LinearLayout>
</ScrollView>
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    android:background="#A34641"
    android:padding="16dp"
    tools:context=".ThankYouActivity">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        android:background="#2E8B8B"
        android:gravity="center_horizontal">

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:background="@android:color/white"
            android:padding="8dp">

            <ImageView
                android:layout_width="200dp"
                android:layout_height="60dp"
                android:layout_alignParentStart="true"
                android:src="@drawable/saveetha_logo_header"
                android:contentDescription="@string/saveetha_logo_affiliate" />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_alignParentEnd="true"
                android:layout_centerVertical="true"
                android:text="TNEA CODE\n1216"
                android:gravity="center"
                android:textSize="18sp"
                android:textStyle="bold"
                android:textColor="#3F51B5" />
        </RelativeLayout>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="50dp"
            android:gravity="center_horizontal"
            android:text="@string/thank_you"
            android:textColor="@android:color/black"
            android:textSize="36sp"
            android:textStyle="bold" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_marginTop="32dp"
            android:gravity="center_horizontal"
            android:paddingStart="32dp"
            android:paddingEnd="32dp"
            android:text="@string/we_are_all_eagerly_waiting"
            android:textColor="@android:color/white"
            android:textSize="28sp"
            android:textStyle="italic" />

        <View
            android:layout_width="match_parent"
            android:layout_height="0dp"
            android:layout_weight="1" />

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/contact_us"
            android:textColor="#FF0000"
            android:textSize="32sp"
            android:textStyle="bold"
            android:gravity="center_horizontal"
            android:layout_marginBottom="16dp"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/email"
            android:textColor="#FF00FF"
            android:textSize="24sp"
            android:textStyle="bold"
            android:gravity="center_horizontal"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/saveethaengineeringcollege_gmail_com"
            android:textColor="#FFFF00"
            android:textSize="20sp"
            android:gravity="center_horizontal"
            android:autoLink="email"
            android:paddingBottom="16dp"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/phone"
            android:textColor="@android:color/black"
            android:textSize="24sp"
            android:textStyle="bold"
            android:gravity="center_horizontal"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/_6311199090"
            android:textColor="#00FFFF"
            android:textSize="20sp"
            android:gravity="center_horizontal"
            android:autoLink="phone"/>

        <TextView
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="@string/_634565980"
            android:textColor="#00FFFF"
            android:textSize="20sp"
            android:gravity="center_horizontal"
            android:autoLink="phone"
            android:paddingBottom="40dp"/>
            
    </LinearLayout>
</LinearLayout>
```

## OUTPUT:

![alt text](../vijay/figmaapp/static/1.png)

![alt text](../vijay/figmaapp/static/2.png)

![alt text](../vijay/figmaapp/static/3.png)

![alt text](../vijay/figmaapp/static/4.png)



## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
