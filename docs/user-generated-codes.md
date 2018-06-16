Please see full documentation at [https://cobrowse.io/docs](https://cobrowse.io/docs).

Try our **online demo** at the bottom of our homepage at <https://cobrowse.io/#tryit>.

## User-generated codes (optional)

These are the native-side requirements on Android to initiate sessions using 6-digit codes. More info at <https://cobrowse.io/docs#user-generated-codes>

You may expose a small UI in your app for users to generate a 6-digit code that they pass to an agent over the phone or chat to initiate a session.

We have provided some default UI to make things easier to get started:

```java
import io.cobrowse.ui.CobrowseActivity;

public class YourActivity extends Activity {

    // the rest of your Activity

    public void startCobrowse(View view) {
        Intent intent = new Intent(this, CobrowseActivity.class);
        startActivity(intent);
    }
}
```

Make sure you've hooked up a trigger for the `startCobrowse` method that we've just added. Then head to <https://cobrowse.io/dashboard> and enter the 6 digit code that will be generated by your app when you trigger the action!

## Questions?
Any questions at all? Please email us directly at [hello@cobrowse.io](mailto:hello@cobrowse.io).