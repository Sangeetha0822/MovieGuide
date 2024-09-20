 ##Project Title: MovieGuide
 
 ## Overview of the Project:
   Movieguide is an Android app that lists popular and highest-rated movies, displays trailers, and shows user reviews. Built using the MVP pattern, RxJava, Dagger 2, and Uncle Bob Martin's Clean Architecture approach, the app is optimized for tablets and demonstrates key architectural concepts. This project is an updated version of a 7-year-old GitHub project.

## Features:
  - Browse popular and top-rated movies
- Watch trailers for movies
- Read and display user reviews
- Optimized UI for tablets

## Technologies Used:
 - MVP (Model-View-Presenter) architecture
- RxJava for reactive programming
- Dagger 2 for dependency injection
- Retrofit for network calls
- Room Database for local data storage
  

## Necessary Changes Made to the Movieguide Project Functional

1. Dependency Updates:

Updated RxJava to version 3.x.x, ensuring compatibility with the latest Android APIs.
Updated Dagger 2 to the latest version and modified dependency injection code accordingly.
Updated Retrofit for network requests, ensuring it uses modern HTTP request handling mechanisms.
Updated the Room database library to the latest version to maintain compatibility with the updated project.

2. Resolved Duplicate Items in Movie Listings:

The issue of duplicate items in the movie listing was addressed by applying RxJava’s distinctUntilChanged() operator. This ensures that only unique movies are displayed.
Further checks were implemented at the repository layer to prevent duplicate data from being returned from the API.

3. Deprecated Code Refactoring:

Replaced outdated AsyncTask with Kotlin coroutines to handle asynchronous tasks.
Refactored old lifecycle methods to use Android Jetpack's ViewModel and LiveData, making the code lifecycle-aware and robust against configuration changes.
Migrated to AndroidX libraries to modernize the code and maintain compatibility with the latest Android development standards.


