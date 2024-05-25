How to grab favicon from websites using js?
Favicon is related to particular website. and displayed in title bar of browser. it is also called shortcut icon
website icon or tab icon. To add favicon in webpage, we need to add syntax in html file (link rel=shortcut icon href="imagename.extension"). 
preferred size is 16x16 and 32x32. preferred type is ico and png. 

Why to add favicon in webpage? benefits? it helps in seo. also user can identify website uniquely. 
we use api of duckduckgo and google for grabbing icon. 
1 api is duckduckgo, to get original sized favicon of any url. api url is https://icons.duckduckgo.com/ip3/Desiredurl.ico.
e.g., https://icons.duckduckgo.com/ip3/apkwires.com.ico

2 api is google api. https://s2.googleusercontent.com/s2/favicons?
it needs 2 parameters. domain (url of website) and sz (size of website).
for ecample, https://s2.googleusercontent.com/s2/favicons?domain=https://www.google.com&sz=32. (if we need size of 16x16,
then we will write sz=16 instead of 32). we can also get of custom size like 64 or else.

we will need to get input from user (url) of which they want to grab icon. they also need to give size or we 
can use default size. 
textbox to get url input and dropdown menu to select the size. 

Learn how to create basic html structure. create html, js file and how to use js file in html document. 

how to create button, how to call function on the click of button, how to show output.
create button, create a function that will show output on clicking the button. 

Learn how to access element using js. 

we can also access image by using .src instead of .value and change the image using js when button is clicked.

by default an image is empty. create select option that will choose one of four options. on selecting one of the first 3 options it will show 
image of related website but if select 4 option it will show invalid input. 
use if else conditions. first create variable and store selected value in it. and compare the value and show related output.

how to validate url using js? we will use function check whether anything input is valid or not. 
create a function and write string in its parameter. use match() method and pass validator string in this 
function to match input with url validater. 
This function will respond if value is not null. 

now create another function to check the url. create another variable to get the value of input and pass this to the 
above validurl function to verify. 
var targettext= document.getelementbyid("id").value;
 alert (isvalidurl(targettext)); call check function, This will show that result is valid or not in alert of website. 

--------------------------------------------------

    <script type="text/javascript">

function isvalidURL(string) {

    var res= string.match(/^(https?:\/\/)?([\w-]+\.)+[\w-]+(\/[\w- .\/?%&=]*)?$/);
    return (res != null)

}

function checkIt() {
    var targettext = document.getElementById("atext").value;
    alert(isvalidURL(targettext));
}

    </script>

<input type="text" id="atext">
<input type="submit" value="click me" onclick="checkIt()">
----------------------------------------------------------------------------------------

Now we will use google and duckduckgo api to fetch favicon. 
first create a dropdown to select the size. give different option and one is default so it will grab according 
to default size of favicon. use input to get url from user and click button on clicking which we can grab icon. 
we use js function for this. 

comments added in index file with each code.

----
at last, host this website free at blogger. 