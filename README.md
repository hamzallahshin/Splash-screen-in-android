# Splash-screen-in-android
How to add splash screen in your android app Here is the code 
      just put the following lines to your Java file and give it some seconds i gave it 4 second and its equal to 4000 



public class SplashScreen extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_crate_account);

         new Handler().postDelayed(new Runnable() {
             @Override
             public void run() {
                 Intent intent=new Intent(SplashScreen.this,MainActivity.class);
                 startActivity(intent);

             }
         },4000);
    }
}



