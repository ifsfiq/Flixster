# Flix
Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED (10pts)

- [X] (8pts) Expose details of movie (ratings using RatingBar, popularity, and synopsis) in a separate activity.
- [X] (2pts) Allow video posts to be played in full-screen using the YouTubePlayerView.

#### BONUS

- [ ] Implement a shared element transition when user clicks into the details of a movie (1 point).
- [ ] Trailers for popular movies are played automatically when the movie is selected (1 point).
  - [ ] When clicking on a popular movie (i.e. a movie voted for more than 5 stars) the video should be played immediately.
  - [ ] Less popular videos rely on the detailed page should show an image preview that can initiate playing a YouTube video.
- [ ] Add a play icon overlay to popular movies to indicate that the movie can be played (1 point).
- [ ] Apply data binding for views to help remove boilerplate code. (1 point)
- [ ] Add a rounded corners for the images using the Glide transformations. (1 point)
- [X] Change UI background color for all screens.
- [X] Change text color for the MainActivity UI screen.
- [X] Change text color and size in DetailActivity UI screen.
- [X] Add two text views as labels for release date and overview, change text color, size and font for those text views.
- [X] Add release date of movie in DetailActivity UI screen.
- [X] Change color of stars to purple in rating bar.

### App Walkthough GIF

<img src="walkthrough2.gif" width=250><br>

### Notes

Describe any challenges encountered while building the app.
A challenge that I faced during building this app was that I tried to implement the stretch story of "Add a rounded corners for the images using the Glide transformations" and it did not work. I was not getting results and it was not working. If I had more time to work on this project, I would look more into completing this stretch story. Another problem that I faced when I was building the app was that in the beginning, my emulator would not work. It would show up but Android Studio would not recognize it and it would cause an error which lead to the emulator not being launched successfully. This meant that the app was not working properly on the emulator as well. I fixed this problem by creating a new emulator and running the app again. Then the new emulator worked properly after that. 

## Open-source libraries used
- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Android


---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [X] (10pts) User can view a list of movies (title, poster image, and overview) currently playing in theaters from the Movie Database API.

#### BONUS
- [X] (2pts) Views should be responsive for both landscape/portrait mode.
   - [X] (1pt) In portrait mode, the poster image, title, and movie overview is shown.
   - [X] (1pt) In landscape mode, the rotated alternate layout should use the backdrop image instead and show the title and movie overview to the right of it.

- [ ] (2pts) Display a nice default [placeholder graphic](https://guides.codepath.org/android/Displaying-Images-with-the-Glide-Library#advanced-usage) for each image during loading
- [ ] (2pts) Improved the user interface by experimenting with styling and coloring.
- [ ] (2pts) For popular movies (i.e. a movie voted for more than 5 stars), the full backdrop image is displayed. Otherwise, a poster image, the movie title, and overview is listed. Use Heterogenous RecyclerViews and use different ViewHolder layout files for popular movies and less popular ones.

### App Walkthough GIF

<img src="walkthrough.gif" width=250><br>

GIF created with [LiceCap](http://www.cockos.com/licecap/).

### Notes
Describe any challenges encountered while building the app.
Some challenges that I encoutered while building this app, were that when trying to make the poster picture wider for the landscape orientation, I had trouble with the formatting 
because when I would change the width of the pciture, it would squish my all of my textViews to the right and it did not look good on the emulator. To fix this, in item_movie.xml
file, I had to chnage the height of my RelativeLayout to wrap_content and not to match_parent which is what I had originally. I also had trouble auto rotating my emulator
whenever I changed the orientation. To fix this, I went to settings and enabled the auto rotate option. Then, finally, I had trouble making a connection from android studio
to the Movie Database API. To fix this, I uninstalled the app from the emulator and then ran the program again. 

### Open-source libraries used

- [Android Async HTTP](https://github.com/codepath/CPAsyncHttpClient) - Simple asynchronous HTTP requests with JSON parsing
- [Glide](https://github.com/bumptech/glide) - Image loading and caching library for Androids
