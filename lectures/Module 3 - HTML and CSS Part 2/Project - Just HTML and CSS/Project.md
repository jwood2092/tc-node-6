# CSS FlexBox & Grid

Goal:


![alt_text](images/image1.png "image_tooltip")



## Part 1

Creating a folder, files, and git repo in the terminal



1. Open your terminal and type -> _cd repos_ -> This will change our current directory to our repos folder.
2. Now that we're inside our repos folder let's type -> mkdir flexboxAndGrid -> This will create the folder where our FlexBox and Grid project will live.
3. Now type -> cd flexboxAndGrid -> This will change our current directory to our FlexBox and Grid project.
4. Next type -> git init -> This will initialize an empty (local) git repository.
5. Now create a blank html file
    1. If you're on the Window's Command Prompt type -> echo " " > index.html -> This will create a blank file inside of our project folder.
    2. If you're on Git Bash or Mac's Terminal type -> touch index.html -> This will create a blank file inside of your project folder.
6. Now create a blank css file 
    3. If you're on the Window's Command Prompt type -> echo " " > index.css -> This will create a blank css file inside of our project folder.
    4. If you're on Git Bash or Mac's Terminal type -> touch index.css -> This will create a blank css file inside of your project folder.


## Part 2

Open VSC and start in index.html



1. Next (Still in your terminal / command prompt / or Git Bash) type -> _code ._ -> This will open an instance of VS Code at your current directory (In our case, the "flexboxAndGrid" folder).
    1. If “code .” doesn’t work, then open up VS Code and click on “Open folder”. Then select your portfolio folder inside of your repos folder.
2. Click on the index.html file on the left side of the VS Code window.
3. Next, click inside of the file and type ->_ ! _-> then press "enter" on your keyboard. This will generate the following HTML Template.


![alt_text](images/image2.gif "image_tooltip")


Create the structure for our KenKen board



1. Inside of the body tag, create a new div with create a div element and add a class name “wrappers”

    1. Type -> &lt;div class=”wrapper”>&lt;/div>
2. Inside of the new div tag, create 16 div elements with span elements as child elements. Give each div a unique id for box and number. Add an “answer” class name and “contenteditable” attribute to the span elements

    2. Type -> &lt;div id=”box1”>&lt;span class=”answer” contenteditable>&lt;/span>&lt;/div>
3. For boxes 1, 3, 5, 7, 9, 12, and 13, add the following spans:

    3. Box1 -> &lt;span class="prompt">8X&lt;/span>
    4. Box3 -> &lt;span class="prompt">4+&lt;/span>
    5. Box5 -> &lt;span class="prompt">10+&lt;/span>
    6. Box7 -> &lt;span class="prompt">4X&lt;/span>
    7. Box9 -> &lt;span class="prompt">1&lt;/span>
    8. Box12 -> &lt;span class="prompt">11+&lt;/span>
    9. Box13 -> &lt;span class="prompt">3+&lt;/span>
4. Your HTML file should now resemble:



![alt_text](images/image3.png "image_tooltip")



## Part 3 

Style the HTML document to resemble the KenKen board



1. Inside your index.css file, add a rule set that applies to the body element. Add:

    1.  _width_: fit-content;
    2.  _height_: fit-content;
    3.  _margin_: 3rem auto;
    4.  _padding_: 0;
    5.  _background-color_: burlywood;

2. Add a rule set that applies to the child divs in the .wrapper element:

    6.  _position_: relative;
    7.  _background-color_: lightblue;
    8.  _font-size_: 3rem;
    9.  _display_: flex;
    10.  _justify-content_: center;
    11.  _align-items_: center;

3. Add a rule set that applies to the .prompt spans:

    12.  _position_: absolute;
    13.  _left_: 0;
    14.  _top_: 0;

4. Add a rule set that applies to the .answer spans:

    15.  _width_: 50%;
    16.  _height_: 50%;
    17.  _text-align_: center;

5. Add a rule set that applies to the .wrapper div:

    18.  _width_: 800px;
    19.  _height_: 800px;
    20.  _display_: grid;
    21.  _grid-template-rows_: repeat(4, 1fr);
    22.  _grid-template-columns_: repeat(4, 1fr);

6. Add a rule set that applies to the divs with ids box1 and box3:

    23.  _border-left_: 3px solid black;
    24.  _border-top_: 3px solid black;
    25.  _border-bottom_: 3px solid black;

7. Add a rule set that applies to the divs with ids box1, box3, box5, box7, box13 and box15:

    26.  _border-right_: 1px solid gray;

8. Add a rule set that applies to the divs with the ids box10, box11 and box16:

    27.  _border-top_: 1px solid gray;

9. Add a rule set that applies to the divs with the ids box2 and box4:

    28.  _border-right_: 3px solid black;
    29.  _border-top_: 3px solid black;
    30.  _border-bottom_: 3px solid black;

10. Add a rule set that applies to the divs with the id box5:

    31.  _border-left_: 3px solid black;
    32.  _border-top_: 3px solid black;
    33.  _border-bottom_: 3px solid black;

11. Add a rule set that applies to the divs with the id box6:

    34.  _border-top_: 3px solid black;
    35.  _border-right_: 3px solid black;

12. Add a rule set that applies to the divs with the id box7:

    36.  _border-top_: 3px solid black;
    37.  _border-left_: 3px solid black;

13. Add a rule set that applies to the divs with the id box8:

    38.  _border-top_: 3px solid black;
    39.  _border-right_: 3px solid black;
    40.  _border-bottom_: 3px solid black;

14. Add a rule set that applies to the divs with the id box10 and box11:

    41.  _border-left_: 3px solid black;
    42.  _border-right_: 3px solid black;
    43.  _border-bottom_: 3px solid black;

15. Add a rule set that applies to the divs with the id box13 and box15:

    44.  _border-left_: 3px solid black;
    45.  _border-bottom_: 3px solid black;
    46.  _border-top_: 3px solid black;

16. Add a rule set that applies to the divs with the id box14:

    47.  _border-right_: 3px solid black;
    48.  _border-bottom_: 3px solid black;
    49.  _border-top_: 3px solid black;

17. Add a rule set that applies to the divs with the id box16:

    50.  _border-bottom_: 3px solid black;
    51.  _border-right_: 3px solid black;


## Part 4

Create a media query for responsive styling



1. Add a media query that applies for screen and max-width: 600px:

    1. @media screen and (_max-width_: 600px) {}

2. Add a rule set for the .wrapper div:

    2.    _width_: 100vw;
    3.    _height_: 100vw;

3. Add a rule set for the .wrapper div’s child divs:

    4.  _font-size_: 1rem;

4. Add a rule set for the .answer spans:

    5.    _width_: 3rem;
    6.    _height_: 3rem;
    7.    _text-align_: center;
    8.    _font-size_: 1.5rem;

	

Awesome! You've just completed the FlexBox and Grid CSS exercise and practiced responsive styling. There’s more to come, so let’s keep going!


# **[Project WalkThrough Video ](https://vimeo.com/563402230)**
