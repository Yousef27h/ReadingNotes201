# Forms

The best known form on the web is probably the search box that sits right in the middle of Google's homepage.

There are several types of form controls that you can use to collect information from visitors to your site.

* ADDING TEXT
* Making Choices
* Submitting Forms
* Uploading Files

A user fills in a form and then presses a button to submit the information to the server.

![Form](/img/form1.JPG)

A form may have several form controls, each gathering different information. The server needs to know which piece of inputted data corresponds with which form element.

```
<form action="http://www.example.com/subscribe.php" method="get">
    <p>This is where the form controls will appear.
    </p>
</form>
```

Form controls live inside a __form__ element. This element should always carry the actionattribute and will usually have a method and id attribute too.

Every form element requires an __action__ attribute. Its valueis the URL for the page on the server that will receive the information in the form when it is submitted.

```
<form action="http://www.example.com/login.php">
    <p>Username:
        <input type="text" name="username" size="15" maxlength="30" />
    </p>
</form>
```
The **input** element is used to create several different form controls. The value of the typeattribute determines what kind of input they will be creating.

When the type attribute has a value of text, it creates a singleline text input.

When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. They are hidden in this way so that if someone is looking over the user's shoulder, they cannot see sensitive data such as passwords.

If you want to allow users to upload a file (for example an image, video, mp3, or a PDF), you will need to use a file input box.

A drop down list box (also known as a select box) allows users to select one option from a drop down list. 

```
<form action="http://www.example.com/profile.php">
    <p>What device do you listen to music on?</p>
    <select name="devices">
        <option value="ipod">iPod</option>
        <option value="radio">Radio</option>
        <option value="computer">Computer</option>
    </select>
</form>
```

The __option__ element is used to specify the options that the user can select from. The words between the opening and closing option tags will be shown to the user in the drop down box.

