# AndroidMVVMTemplate

This template is setup with the basic MVVM package structure with common dependencies already in the gradle files.

Project gradle added dependendy:
  classpath "com.google.dagger:hilt-android-gradle-plugin:2.38.1"
  
Build gradle additions:
  plugins:
    id 'kotlin-kapt'
    id 'dagger.hilt.android.plugin'
    
  defaultConfig:
    buildConfigField 'String', 'BASE_URL', "\"Add Base URL here\""
    
  buildFeatures:
    viewBinding true
    dataBinding true
    
  dependencies:
    implementation 'androidx.fragment:fragment-ktx:1.3.6'

    // Retrofit
    implementation 'com.squareup.retrofit2:retrofit:2.9.0'
    implementation 'com.squareup.retrofit2:converter-moshi:2.9.0'

    // Moshi
    implementation 'com.squareup.moshi:moshi-kotlin:1.12.0'
    implementation 'androidx.legacy:legacy-support-v4:1.0.0'
    kapt 'com.squareup.moshi:moshi-kotlin-codegen:1.12.0'

    // OKHttp
    implementation 'com.squareup.okhttp3:logging-interceptor:4.9.1'

    // Hilt
    implementation "com.google.dagger:hilt-android:2.38.1"
    kapt "com.google.dagger:hilt-android-compiler:2.38.1."

    // Navigation
    implementation 'androidx.navigation:navigation-fragment-ktx:2.3.5'
    implementation 'androidx.navigation:navigation-ui-ktx:2.3.5'

    // Coroutines
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-core:1.5.1'
    implementation 'org.jetbrains.kotlinx:kotlinx-coroutines-android:1.5.1'

    // Glide
    implementation 'com.github.bumptech.glide:glide:4.12.0'
    kapt 'com.github.bumptech.glide:compiler:4.12.0'
 

Feel free to clone and utilize this repository.
