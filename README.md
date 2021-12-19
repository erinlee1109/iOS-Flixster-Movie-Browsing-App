# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

### User Stories

- [x] User sees an app icon on the home screen and a styled launch screen.
- [x] User can view and scroll through a list of movies now playing in theaters.
- [x] User can view the movie poster image for each movie.
- [x] User can tap a cell to see more details about a particular movie.
- [x] User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.


### App Walkthrough GIF
<img src="http://g.recordit.co/Pf0eng5LG7.gif" width=250><br>

<img src="https://recordit.co/atMrATKQzW.gif" width=250><br>

### Challenge
Installing AlamofireImage has been a huge unexpected challenge. 
Even after cleaning the build and re-building, manually building the framework, 
and deleting the 'derived data' folder, I was still receiving 100+ errors on Xcode, 
mainly two errors: "Could not build Objective-C module 'AlamofireImage'" and 
"No such module 'AlamofireImage'". 
The solution was to specify the version in the Podfile. For my specific case, I add the following, 
and Alamofire (4.9.1) and AlamofireImage (3.6.0) were installed instead.  
```
#Pods for flixster
pod 'AlamofireImage', '~> 3.1'
```
