# Android-Register

![Register Capture](https://user-images.githubusercontent.com/3745464/100115217-4146d580-2e98-11eb-8bd1-0cfb1dde211a.PNG)

Try material Register xml design

Android Register Screen

XML layout design for android

Android Material login screen with androidx dependency

buildToolsVersion 30.0.1

minSdkVersion 14

    implementation 'com.google.android.material:material:1.0.0'
    implementation 'androidx.cardview:cardview:1.0.0'


XML:

<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@color/colorPrimary"
    tools:context=".MainActivity">
    <ImageView
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:scaleType="fitEnd"
        app:srcCompat="@drawable/bg_wave"/>
    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="match_parent">
        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="match_parent"
            android:gravity="center"
            android:orientation="vertical">
           <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:paddingBottom="20dp"
                android:orientation="vertical">
                <androidx.cardview.widget.CardView
                    android:id="@+id/cv"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_margin="10dp"
                    android:clickable="true"
                    android:foreground="?attr/selectableItemBackgroundBorderless"
                    app:cardCornerRadius="20dp"
                    app:cardElevation="10dp"
                    app:cardPreventCornerOverlap="false"
                    app:cardUseCompatPadding="false">
                    <RelativeLayout
                        android:layout_width="match_parent"
                        android:layout_height="wrap_content">
                        <LinearLayout
                            android:layout_width="match_parent"
                            android:layout_height="wrap_content"
                            android:orientation="vertical">
                            <TextView
                                android:id="@+id/listText"
                                android:layout_width="match_parent"
                                android:layout_height="wrap_content"
                                android:layout_gravity="center_horizontal"
                                android:padding="8dp"
                                android:text="Register"
                                android:gravity="center"
                                android:textColor="@color/colorPrimary"
                                android:textSize="30dp" />
                            <LinearLayout
                                android:id="@+id/linearLayout"
                                android:layout_width="match_parent"
                                android:layout_height="wrap_content"
                                android:orientation="vertical"
                                android:layout_margin="10dp"
                                android:padding="15dp">
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">

                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/fname"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="text"
                                        android:hint="First Name" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">

                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/lname"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="text"
                                        android:hint="Last Name" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <LinearLayout
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:orientation="horizontal">
                                    <TextView
                                        android:layout_width="wrap_content"
                                        android:layout_weight="1"
                                        android:layout_margin="5dp"
                                        android:layout_height="wrap_content"
                                        android:text="Select Gender"/>

                                    <RadioGroup
                                        android:id="@+id/radioSex"
                                        android:layout_width="wrap_content"
                                        android:layout_height="wrap_content" >

                                        <RadioButton
                                            android:id="@+id/radioMale"
                                            android:layout_width="wrap_content"
                                            android:layout_height="wrap_content"
                                            android:text="Male"
                                            android:checked="true" />

                                        <RadioButton
                                            android:id="@+id/radioFemale"
                                            android:layout_width="wrap_content"
                                            android:layout_height="wrap_content"
                                            android:text="Female" />

                                    </RadioGroup>
                                </LinearLayout>

                                <LinearLayout
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:gravity="center_vertical"
                                    android:orientation="horizontal">

                                    <TextView
                                        android:id="@+id/textView3"
                                        android:layout_width="wrap_content"
                                        android:layout_height="wrap_content"
                                        android:layout_alignRight="@+id/button1"
                                        android:layout_below="@+id/textView2"
                                        android:layout_marginTop="5dp"
                                        android:layout_weight="1"
                                        android:text="Date of Birth"
                                        android:textAppearance="?android:attr/textAppearanceMedium" />
                                    <androidx.appcompat.widget.AppCompatButton
                                        android:id="@+id/dob"
                                        style="@style/AppTheme.RoundedCornerMaterialButton"
                                        android:layout_width="wrap_content"
                                        android:layout_height="wrap_content"
                                        android:layout_weight="1"
                                        android:padding="10dp"
                                        android:text="Select Date of Birth "
                                        android:textColor="@color/colorPrimary"
                                        android:textColorHint="#348FFF" />
                                </LinearLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">

                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/email"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="textWebEmailAddress"
                                        android:hint="Email ID" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">
                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/mobile"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="number"
                                        android:hint="Mobile Number" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">
                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/address"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="textWebEmailAddress"
                                        android:hint="Address" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">

                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/city"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="text"
                                        android:hint="City" />
                                </com.google.android.material.textfield.TextInputLayout>

                                <LinearLayout
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:gravity="center_vertical"
                                    android:orientation="horizontal">
                                    <TextView
                                        android:layout_width="match_parent"
                                        android:layout_weight="1"
                                        android:layout_margin="5dp"
                                        android:layout_height="wrap_content"
                                        android:text="Select State"/>
                                    <Spinner
                                        android:id="@+id/state"
                                        android:layout_weight="1"
                                        android:layout_margin="5dp"
                                        android:padding="6dp"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content" />
                                </LinearLayout>
                                <com.google.android.material.textfield.TextInputLayout
                                    style="@style/Widget.MaterialComponents.TextInputLayout.OutlinedBox"
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content">
                                    <com.google.android.material.textfield.TextInputEditText
                                        android:id="@+id/pin"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content"
                                        android:inputType="textWebEmailAddress"
                                        android:hint="Pin Code" />
                                </com.google.android.material.textfield.TextInputLayout>
                                <LinearLayout
                                    android:layout_width="match_parent"
                                    android:layout_height="wrap_content"
                                    android:orientation="horizontal">
                                    <TextView
                                        android:layout_width="match_parent"
                                        android:layout_weight="1"
                                        android:layout_margin="5dp"
                                        android:layout_height="wrap_content"
                                        android:text="Select Country"/>
                                    <Spinner
                                        android:id="@+id/country"
                                        android:layout_weight="1"
                                        android:layout_margin="5dp"
                                        android:padding="6dp"
                                        android:layout_width="match_parent"
                                        android:layout_height="wrap_content" />
                                </LinearLayout>
                                <TextView
                                    android:layout_width="match_parent"
                                    android:background="@color/colorAccent"
                                    android:layout_height="1dp"
                                    android:textStyle="bold"
                                    android:layout_marginTop="15dp"
                                    android:text=""/>
                            </LinearLayout>
                        </LinearLayout>
                    </RelativeLayout>
                </androidx.cardview.widget.CardView>
            </LinearLayout>
            <androidx.appcompat.widget.AppCompatButton
                android:id="@+id/buttonAwesomeqw"
                style="@style/AppTheme.RoundedCornerMaterialButton"
                android:layout_width="150dp"
                android:layout_height="wrap_content"
                android:layout_marginTop="-60dp"
                android:padding="10dp"
                android:text="Register"
                android:textColor="@color/colorPrimary"
                android:textColorHint="#348FFF" />
            <Button
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                style="@style/Widget.AppCompat.Light.ActionButton.CloseMode"
                android:text="Cancel"
                android:textAllCaps="false" />
        </LinearLayout>
    </ScrollView>
</RelativeLayout>
