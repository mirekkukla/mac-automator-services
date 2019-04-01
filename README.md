## About

Service scripts for built-in mac [automator](https://support.apple.com/guide/automator/welcome/mac) app. Services are "scripts" of sorts that you can trigger when right-clicking on the appropriate context (such as highlighted text or a file in finder).

## Usage

To add a service in this repo copy the desired service folder from `~/Library/Services`

To "install" a given service simply double-click the outer "<name>.workflow" file and it will open in automator and prompt you to install it.

## Services

#### Resize image to 1920
Right-click an image and resize it to 1920 x (whatever keeps the ration constant). Is useful when you have an image you might want to upload to a website. The vast majority of screens will dedicate less than 1920 pixels to any given image, and by reducing the pixel count you significantly reduce the size.

#### Extract Email Addresses.workflow
Right-click a section of highlighted text and extract all things that look like email adresses from it.

#### Extract Email Addresses.workflow
After you've copied some text in the Mac kindle app, use this workflow to replace the contents of your clipboard with a variant of the copied texts surrounded in quotes and only has the page number (instead of the entire MLA citing).
* Create a keyboard shortcut for the service (I useed [option]+[command]+k [for "kindle"]). The workflows is then: 1) copy the text, 2) press the keyboard shortcut, 3) paste the text.
* You should see a notififcation pop up notifying you if the action worked / was ignored (which happens if the clipboard contents is deemed to not have been copied from the kindle app).
* Example: clipboard contents before and after workflow
    ```
    Zazen practice is the practice in which we resume our pure way of life

    Suzuki, Shunryu. Zen Mind, Beginner's Mind (pp. 115-116). Shambhala. Kindle Edition.
    ```
    ```
    "Zazen practice is the practice in which we resume our pure way of life" (115-116)
    ```
