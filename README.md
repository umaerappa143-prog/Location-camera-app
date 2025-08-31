# Location-camera-app
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout 
   xmlns:android="http://schemas.android.com/apk/res/android"
   xmlns:app="http://schemas.android.com/apk/res-auto"
   android:layout_width="match_parent"
   android:layout_height="match_parent">

    <androidx.camera.view.PreviewView
        android:id="@+id/viewFinder"
        android:layout_width="0dp"
        android:layout_height="0dp"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintBottom_toTopOf="@id/locationLayout"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintEnd_toEndOf="parent"/>

    <LinearLayout
        android:id="@+id/locationLayout"
        android:orientation="vertical"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:layout_constraintBottom_toBottomOf="parent"
        android:padding="16dp"
        android:background="#AA000000">

        <TextView android:id="@+id/latitudeText"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Latitude: "/>

        <TextView android:id="@+id/longitudeText"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Longitude: "/>

        <Button 
            android:id="@+id/showLocationMapButton"
            android:layout_width="wrap_content"
            android:layout_height="wrap_content"
            android:text="Show Location on Map"/>

    </LinearLayout>
</androidx.constraintlayout.widget.ConstraintLayout>


