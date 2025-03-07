# CustomImports
This repository is mostly to hold the modules that my [Custom Chattriggers Jar](https://github.com/DocilElm/ChatTriggers/releases/tag/2.2.1) can use to import modules.

# Manually Installing
If you are here to manually install the modules rather than using the Jar then this section is for you.<br>

## Step 1
In this repository you can find modules that you want to install, you can click on the folder of the module go into the `download.zip` file click on it and proceed to click on `view raw` which will trigger a downloading of said zip file.

## Step 2
Once you have your zip file you can go back to the normal folder of the module, there you will find a `metadata.json` file this file is important because it'll tell us the dependencies that the module we want to install requires to work properly.

## Step 3
Inside of the `metadata.json` file you _should_ see a `requires` part, this part states the modules that it depends on to work properly.<br>
NOTE: If the `metadata.json` does not contain a `requires` this means that the module does not depend on any other to work properly.<br>

## Step 4
(Skip this step if it does not contain a `requires`).<br>
Having all the modules that it depends on we can now go and repeat Step 1 and so on to install them.

## Step 5
Once we have all the dependencies and module that we want to install we'll head over to all the zip files that we now have and unzip each one of them. There should be a folder inside of the unzipped/extracted zip that is called the same as the module that you are trying to install.

## Step 6
Having every single folder we can now go in game and type the command `/ct files` then hit enter, a file explorer should pop up now we go inside of the folder that is called `modules`.

## Step 7
Paste all your folders that were inside of each unzipped/extracted zip file.

## Step 8
Go back in game and type `/ct load` then hit enter.

## Step 9
If all done correctly the module that you wanted to install should work properly.

## Step 10
If you are dumb enough to get to this step that means that you did something wrong and thus this step was made to help you attempt to debug the issue.

### Step 10.1
If the module did not work properly you should go back in game and type `/ct console js` then hit enter, a console-like window should pop up.

### Step 10.2
You should now see an error/red text inside of this console. The error should look something like this `org.mozilla.javascript.JavaScriptException: Error: Module "<ModulesFolderPath>/Vigilance/index" not found. (<ModulesFolderPath>/Coleweight/settings.js#1)`.<br>
Obviously the error should name the module that you are attempting to install it will for obvious reasons not be `Vigilance` or `Coleweight` as it's in the example text.

### Step 10.3
With this in mind you can see that the first module path contains the module name which in this case it's `Vigilance`, and the error says that it could not find the module so that means that you did not install the dependencies correctly, so you may now go and install that dependency that is telling you it's missing.

### Step 10.4
Repeat this cycle until you no longer get any errors, then try out the module it should work out.<br>
If you are getting a different error go into the `#help` channel in ChatTriggers discord and paste it there, we'll happily help you.

# Is It Safe?
I am part of the team in chattriggers that verifies module releases to not have any malicious code in them before being accepted, all of these i have manually gone through to make sure they are safe.
