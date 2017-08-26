# nbb


allprojects {
    repositories {
        jcenter()
        maven {
            url "https://maven.google.com"
        }
    }
}

package ...
import ...
import com.google.android.gms.ads.MobileAds;

public class MainActivity extends AppCompatActivity {
    ...
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        // Sample AdMob app ID: ca-app-pub-3940256099942544~3347511713
        MobileAds.initialize(this, "YOUR_ADMOB_APP_ID");
    }
    ...
}
