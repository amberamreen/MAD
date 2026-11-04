# MAD
# "This repository contains my Mobile Application Development (MAD) projects, practical tasks, assignments, and learning activities. It showcases my journey of learning mobile app development and building application development skills."
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <ScrollView
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:fillViewport="true"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:orientation="vertical"
            android:padding="16dp">

            <TextView
                android:id="@+id/textView"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/hello_world" />

            <Button
                android:id="@+id/button"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="@string/button_test" />

            <EditText
                android:id="@+id/editName"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:autofillHints="name"
                android:drawableStart="@android:drawable/ic_menu_edit"
                android:hint="@string/hint_enter_name"
                android:inputType="textPersonName"
                android:maxLength="30"
                android:maxLines="1" />

            <ImageView
                android:id="@+id/imageProfile"
                android:layout_width="150dp"
                android:layout_height="150dp"
                android:adjustViewBounds="true"
                android:contentDescription="@string/content_desc_profile"
                android:scaleType="centerCrop"
                android:src="@drawable/profile_pic" />

            <CheckBox
                android:id="@+id/checkAgree"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:buttonTint="#2196F3"
                android:checked="false"
                android:text="@string/text_agree_terms" />

            <RadioGroup
                android:id="@+id/genderGroup"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content">

                <RadioButton
                    android:id="@+id/radioMale"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:buttonTint="#FF5722"
                    android:checked="true"
                    android:text="@string/gender_male" />

                <RadioButton
                    android:id="@+id/radioFemale"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:text="@string/gender_female" />

            </RadioGroup>

            <ToggleButton
                android:id="@+id/toggleWifi"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:backgroundTint="#4CAF50"
                android:checked="false"
                android:textOff="@string/toggle_wifi_off"
                android:textOn="@string/toggle_wifi_on" />

            <androidx.appcompat.widget.SwitchCompat
                android:id="@+id/switchBluetooth"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:checked="true"
                android:text="@string/switch_bluetooth"
                android:thumbTint="#FFFFFF"
                android:trackTint="#4CAF50" />

            <ProgressBar
                android:id="@+id/progressLoading"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:indeterminate="true" />

            <ProgressBar
                android:id="@+id/progressDownload"
                style="?android:attr/progressBarStyleHorizontal"
                android:layout_width="200dp"
                android:layout_height="wrap_content"
                android:max="100"
                android:progress="40"
                android:progressTint="#4CAF50" />

            <androidx.recyclerview.widget.RecyclerView
                android:id="@+id/recyclerView"
                android:layout_width="match_parent"
                android:layout_height="200dp"
                android:nestedScrollingEnabled="false"
                android:padding="8dp"
                android:scrollbars="vertical" />

            <Spinner
                android:id="@+id/spinnerCountry"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:entries="@array/country_list"
                android:padding="8dp"
                android:prompt="@string/prompt_select_country"
                android:spinnerMode="dropdown" />

            <ListView
                android:id="@+id/listNames"
                android:layout_width="match_parent"
                android:layout_height="200dp"
                android:dividerHeight="1dp"
                android:nestedScrollingEnabled="false"
                android:padding="8dp" />

            <AutoCompleteTextView
                android:id="@+id/autoCountry"
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:completionThreshold="1"
                android:hint="@string/hint_enter_country"
                android:padding="8dp"
                android:textSize="16sp" />

        </LinearLayout>
    </ScrollView>
</androidx.constraintlayout.widget.ConstraintLayout>
