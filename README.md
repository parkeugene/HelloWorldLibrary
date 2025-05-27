# Hello World Library for Android 
This is a simple "Hello World" library for Android, demonstrating how to create and use a basic library in an Android project.

## Structure
The library is structured as follows:

```
HelloWorldLibrary/
├── build.gradle.kts
├── settings.gradle.kts
├── README.md
└── helloworld/
    ├── build.gradle.kts
    └── src
        └── main
            └── java
                └── kr
                    └── co
                        └── sakak
                            └── haily
                                └── helloworldlibrary
                                    └── HelloWorld.kt
```


## Usage
To use this library in your Android project, follow these steps:

1. Add the library dependency to your `build.gradle.kts` file:
   ```
   dependencies {
    ...
    implementation("com.github.parkeugene:HelloWorldLibrary:1.0.8")
    ...
}
   ```

2. In your activity or fragment, you can use the library as follows:
   ```kotlin
    import kr.co.sakak.haily.helloworldlibrary.HelloWorld
    
    class MainActivity : AppCompatActivity() {
        override fun onCreate(savedInstanceState: Bundle?) {
            super.onCreate(savedInstanceState)
            setContentView(R.layout.activity_main)

            // Use the HelloWorld library
            var greeting = HelloWorld.sayHello()
            Log.d("TAG", greeting)
        }
    }
    
    ```