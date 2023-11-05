# RetrofitMasterclassV2

Retrofit is a powerful open-source library for Android that simplifies the process of making network requests to web services or APIs. It allows you to define type-safe API calls using annotated interfaces, handles request configuration, response parsing, asynchronous operations, and error handling, making it a popular choice for Android app developers. It is often used in conjunction with OkHttp for efficient and reliable network communication.

## Installations
Add the following dependency in module level build gradle file
```
implementation("com.squareup.retrofit2:retrofit:2.9.0")
```

## Mechanism
Retrofit streamlines the integration of web services in Android apps, offering a structured mechanism for handling network requests. This organized approach enhances the efficiency and reliability of communication with external APIs, allowing developers to create robust and scalable applications.

1. Create api interface
2. Create retrofit instance
3. Create api service instance
4. Call api
5. Get data

## Api Interface
In Retrofit, the API interface is a fundamental part of defining and structuring your network requests. It's an interface that specifies the API endpoints, HTTP methods, request parameters, and expected response types.
```kt
// example api interface
interface ApiService{  
    @GET("path/to/your/api")  
    fun data(): Call<ResponseBody>  
}
```

## Retrofit Instance
A Retrofit instance in Android is a central component of the Retrofit library. It serves as the core configuration hub, responsible for defining how network requests are made. When creating a Retrofit instance, you specify essential details such as the base URL of the API, the converter for data serialization and deserialization (typically JSON), and any custom HTTP client settings. This instance acts as the bridge between your API service interface and the actual HTTP requests, ensuring that the requests are made according to your defined settings. By configuring the Retrofit instance appropriately, you can streamline the entire network communication process, making it efficient, robust, and tailored to your application's specific needs.
```kt
val retrofit = Retrofit  
    .Builder()  
    .baseUrl("https://your.site.url")  
    .build()
```

## Api Service Instance
The API service instance in Retrofit is where you put your API interface into action. It connects your defined API endpoints with the actual network requests, making your app's communication with the server possible. It's like the hands-on part of Retrofit that turns your interface into real requests.
```kt
```

<!--stackedit_data:
eyJoaXN0b3J5IjpbMzA1MTczMjIzLDIwODY5NzU1NjksMTY0Nj
kxMzQ3LC03NjgzOTA5NTYsLTIwOTE2NjAzMiwtNjM3MzQ2MDIs
NjgzMTMxMTEwLC0yMjU4OTU1OTEsMTg0NzA1NzkxLC0xOTg0NT
A5Mzk4XX0=
-->