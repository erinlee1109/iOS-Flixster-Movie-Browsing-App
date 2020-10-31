# Flix

Flix is an app that allows users to browse movies from the [The Movie Database API](http://docs.themoviedb.apiary.io/#).

## Flix Part 2

### User Stories

#### REQUIRED (10pts)
- [x] (5pts) User can tap a cell to see more details about a particular movie.
- [x] (5pts) User can tap a tab bar button to view a grid layout of Movie Posters using a CollectionView.

#### BONUS
- [ ] (2pts) User can tap a poster in the collection view to see a detail screen of that movie.
- [ ] (2pts) In the detail view, when the user taps the poster, a new screen is presented modally where they can view the trailer.

### App Walkthrough GIF
<img src="http://g.recordit.co/Pf0eng5LG7.gif" width=250><br>

### Notes
N/A

---

## Flix Part 1

### User Stories

#### REQUIRED (10pts)
- [x] (2pts) User sees an app icon on the home screen and a styled launch screen.
- [x] (5pts) User can view and scroll through a list of movies now playing in theaters.
- [x] (3pts) User can view the movie poster image for each movie.

#### BONUS
- [ ] (2pt) User can view the app on various device sizes and orientations.
- [ ] (1pt) Run your app on a real device.

### App Walkthrough GIF
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
