helloworld代码：

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />




结果：



![image](https://github.com/tujunkun/shiyan1/blob/f7b65f73c6d1fd2f85fd4b3f002e7a808372651c/1.png)



activity代码:

public class MainActivity extends AppCompatActivity {
    public static final String TAG="lifecycle";
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Log.d(TAG,"oncreate");
    }
        @Override
        protected void onStart(){
            super.onStart();
            Log.d(TAG,"onstart");
        }
        @Override
        protected void onResume(){
            super.onResume();
            Log.d(TAG,"onresume");
        }
        @Override
        protected void onPause(){
            super.onPause();
            Log.d(TAG,"onpause");
        }
        @Override
        protected  void onStop(){
            super.onStop();
            Log.d(TAG,"onstop");
        }
        @Override
        protected void onDestroy(){
            super.onDestroy();
            Log.d(TAG,"onDestroy");
        }
        @Override
        protected void onRestart(){
            super.onRestart();
            Log.d(TAG,"onrestart");
        }
}


结果：
        
        
![image](https://github.com/tujunkun/shiyan1/blob/master/2.png)


![image](https://github.com/tujunkun/shiyan1/blob/master/3.png)
