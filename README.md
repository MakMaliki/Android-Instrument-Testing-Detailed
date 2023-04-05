# Android-Instrument-Testing-Detailed

import android.content.Context;

import androidx.test.ext.junit.runners.AndroidJUnit4;
import androidx.test.platform.app.InstrumentationRegistry;

import org.junit.Test;
import org.junit.runner.RunWith;

import static org.junit.Assert.*;

@RunWith(AndroidJUnit4.class)
public class ExampleInstrumentedTest {

    @Test
    public void useAppContext() {
        // Context of the app under test.
        Context appContext = InstrumentationRegistry.getInstrumentation().getTargetContext();

        assertEquals("com.example.myapp", appContext.getPackageName());
    }
}

In this example, we're testing that the context returned by InstrumentationRegistry matches the package name of our app. We're using the AndroidJUnit4 runner to run our test. You can run this test by right-clicking on the class in Android Studio and selecting "Run 'ExampleInstrumentedTest'".
