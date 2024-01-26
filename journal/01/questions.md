# Foundations of Web Development
01. In your own words, why do we use Git?
    > because it makes life easy! we can track projects and the changes we make to them and access previous versions

02. In the terminal, what is the command `mkdir` used for?
    > make directory, makes a folder

03. What is a ***pseudo-class*** and what are some of the most common ones you think you will use?
    > psuedo classes are the ones that come after classes. ex. class:psuedo-class a common use is for a link or button hover effect. ex. 
```css
    a:hover {
        background-color: white;
        text-color: blue;
        border: 2px solid blue; 
    }
```

04. What is ***specificity*** and how might you use it to your benefit?
    > Specificity can be described as how much weight a specific rule will have when applied to an element. #id tags have a weight of 100, class tags have a weight of 10, psuedo-class tags also have a weight of 10 ect, defaults have 0 weight. if any two or more conflicting css rules apply to the same object it uses specificity to determine which rule has the most weight.
```css
    /* corection - I found out that :hover has specificity of 10 while some others like :before and :after just have 1. Not all psuedo-classes are created equal. */
```

05. What problems do you think you could run into if you over-utilized the `!important` feature?
    > YOU ARE MESSING WITH THE NATURAL ORDER OF SPECIFICITY! specificity will be absolute, and having two absolutes would be problematic, not to mention you should just get used to writing your code with natural specificity in mind.

06. What are the three components that makeup a `CSS` rule? <br> Example:
    ```css
        h1 {
            color: rgba(255, 210, 33, .75);
        }
    ```
    the selector 'h1', the property 'color', the value '(255, 210, 33, .75)'

    > | ANSWER HERE |

07. How do you think good design influences people when visiting a website, and what sorts of things could you convey through design alone?
    > Yes. If I see a website with an eye catching color scheme, I will probably spend more time on the website than if the colors are obnoxious. one example is that when I first downloaded the fs-journals it started with a really bright, eye-piercing red that made my eyes hurt. If I saw a website with that color so predominant, I wouldn't want to go back unless I had too.
    if it's user friendly, and everything works with minimal effort, they will continue to see the site as a time saving tool and an asset as well. 

08. What is the purpose of ***wireframing***?
    > to get a plan! an Idea of where the project is going and take it there. outlines position of content and meets the needs of the user before adding the content. 
    I wouldn't put all the text in one main block without any images unless I wanted to make the most boring website in the world. But I still need to know WHERE to put the images. 

09. Do you think wireframes are worth the time, energy, and effort that they require? Why or Why not?
    > In actual application. Yes. A wireframe can be compared to having the picture on the box while building a puzzle. If you are designing multiple pages of content and want to link them together and have them do lots of different things than a wireframe is going to be necessary for building out the web page just like the full image is necessary for matching up the puzzle pieces and knowing when and where to put them. 
    if its a nine piece puzzle or a single web page with no javascript, and especially if you don't need to make it mobile approved. you could very easily get away with not doing a wireframe like everyone did during this first week.

10. Define the display `:flex property:`
    > flex is awesome! it just makes things work. 
    display: block; is the default for most elements and is oriented the top right with a margin that contains the whole line horizontally, with a height of the object. 
    display flex removes the margin horizontally. 
    I was not confident with 'flex' 'justify-content' or 'align-items' until the lily-pap frogs warm-up.

11. What `CSS` properties affect the size of a box model?
    > height and width. 
    padding and margin also have a play in how a box model will interact with other box objects. 

12. Did I wait to do this last minute?
    > Maybe 

13. Should I have done this earlier?
    > Probably

14. Will I do the next one any sooner?
    > Probably not