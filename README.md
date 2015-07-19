# LEGO® Minifigure Head Finder
A web application that allows you to search through all official LEGO® minifigure heads for ones matching a specific criteria. For example, if you are building a scene of red-headed male Vikings and want to find all heads that have red beards but which don't have glasses or any other anachronistic features, this application will enable you to search for heads matching that criteria, which might be an arduous task otherwise.

The app will use the website [BrickLink](http://www.bricklink.com/) to find all available heads, and each head found by a search will have a link back to the original BrickLink entry. I will ask permission from the website to display their images on the app.

Several components will need to be created. The **first** will scan the [Minifig Head](http://www.bricklink.com/catalogList.asp?catType=P&catString=238) listings at BrickLink and create a list of all the item numbers of the minifigure heads. New heads are constantly being added so this will need to add only the items numbers that are not already on the list.

The **second** component will be used by me to create the details for each head in the list. It will check that it is a new entry, and if it is, it will display a picture of the head from BrickLink and their description of the head. I would choose the features from a series of radio buttons, for example, glasses, black eyebrows and no beard, and my selections would be saved to a file. Currently I think a very basic text file would be sufficient, so a new entry and a processed entry might be:

```
3626bpb0596,0
3626bpsc,1,0,1,3,2,1,0,2
```

The first data on each line is the code for the head, the second indicates whether the entry has been processed or not, and the remaining data indicates the details.

The **third** component will be a web page that displays a series of radio buttons and generates a list of minifigure heads based on the options listed, with a link back to the BrickLink entry for each head. This is the only component that the user will see.

As I am a student I expect this small project to take some time, however hopefully if will eventually be useful to the Lego creative community.
