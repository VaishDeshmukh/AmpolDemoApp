## Additional Info:

1. Install homebrew on computer
------> mkdir homebrew && curl -L https://github.com/Homebrew/brew/tarball/master | tar xz --strip 1 -C homebrew

2. Install npm using homebrew
------> brew install node

3. Install json-server using npm 
------> npm install -g json-server
https://github.com/typicode/json-server

4. Create dataBase for the local json on your computer
------> Documents + save file as (db.json)

5. Host it on local using terminal 
------> json -server --watch transaction.json

3. Open any browser & go to 
------> http://localhost:3000/db

Tada !! We have successfully established the connection. Now run the CBA App. It should all go well !! 


## Architecture

1. MVVM is used as the architecture pattern along with SwiftUI & Combine.
2. All common objects are created as a sparate classes.
3. Mapkit is being used to display location of the nearest station.


## Implementation

1. I have added support from iOS 15 & above considering the requirement. It would scale good on Iphone 14 pro.
2. I have designed the app, to show entry point for 3 products as tab view item inside a single view.
3. The data is fetched from the json server hosted on local.
4. Each of the three views are identical which uses the same re-usable view which is populated using relevant viewModel to display the data on UI.
5. I couldn't implement the detail view for the See All items on the view. A sample for transaction view is done.
6. I have added the offers section as a horizontal carousel which gives a good insight of top 3 deals on main page.
7. The Nearby Locations section displays the nearest location of the fuel station. Clicking on it will take user to the mapView with an annotation on the app. Which would intern display an alert with the location detail when tapped on the map annotation.
8. I have added some unit tests around the network layer, given the time limit on the project.
9. I have added independent file for Icons & Colors so it can be used globally throught the app. Given more time we can create a design system library & add it as swift package manager.



## Time Taken

The entire project took over 3 hours of total work. A little bit of ad-hoc touch ups in between.


