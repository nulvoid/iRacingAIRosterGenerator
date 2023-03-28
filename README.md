# iRacing AI Roster Generator
This is a faily simple program written in Python that will generate an AI roster for iRacing. Currently it only supports Late Models and Super Late Models because these are the cars that I used while testing, but I plan on expanding the program to include other oval cars. At this time I do not plan on adding support for road cars simply because I don't own them and I have no interest in them. The Lotus 79 may be added in the future however, because I do enjoy driving it.

To use the program simply just run the .py file. You will be prompted to choose which car class you want, a name for the roster, and how many cars you want in the roster (caps at 60). All required modules should be included with a standard Python installation. Always make sure you install the latest version of Python if you are installing it for the first time.

## Notes

### directory_path
Line 6 of the program specifies the standard iRacing AI roster folder location, and will create the entire file path if this does not exist. If your AI roster folder is in a different location, change the directory to yours.

### colors.txt
colors.txt is a text file containing a list of a group of three hexadecimal color codes seperated by a space. This format was chosen for now to allow the option of picking three colors for the cars that get generated, instead of the program randomly generating three colors and half your field being pink. The supplied colors.txt file may be used, or you can edit it to your liking. While editing it, ensure you follow the following format:
```
FF000A 000000 FFFFFF
2BFD26 FFFFFF 1C9FFD
2A3795 000000 FFFFFF
```
Where line one represents the colors red, black, and white, line two represents the colors blue, white, and blue, and so on.

### first_names.txt
first_names.txt is a text file containing a list of first names. The supplied first_names.txt may be used, or you can edit it to your liking. While editing it, ensure you follow the following format:
```
James
John
Robert
Michael
```
Where every name is on its own line.

### last_names.txt
last_names.txt is a text file containing a list of last names. The supplied last_names.txt may be used, or you can edit it to your liking. While editing it, ensure you follow the following format:
```
Smith 
Johnson 
Williams 
Brown
```
Where every name is on its own line.

# To Do
- [x] Add Late Models
- [x] Add Super Late Models
- [x] Rewrite car class selection to easily allow for the addition of new car classes
- [ ] Add SK Modifieds
- [ ] Add Tour Modifieds
- [ ] \(Optional) Add SK and Tour Modified roster option (Fun at trucks like Oxford)
- [ ] Add Street Stocks
- [ ] Add ARCA
- [ ] Add Legends
- [ ] Add NASCAR Trucks
- [ ] Add NASCAR xFinity
- [ ] Add NASCAR Cup
- [ ] Add NASCAR 87 Cup
- [ ] Add Indycar
- [ ] Write program for generating iRacing seasons
- [ ] Rewrite old version of program that references Github repositories for names and colors
- [ ] Figure out a better way of generating car colors instead of having a database of colors
- [ ] Figure out an easier way of fiding values for things like sponsor ranges and paint scheme ranges than hand making rosters with the first and last options and hoping that the numbers match perfectly
- [ ] GUI
