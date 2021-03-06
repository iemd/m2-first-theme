# Magento 2 First Theme
This is a simple Magento 2 theme to demonstrate how a theme works inside the Magento 2 system and what are those minimum requirements which make a Magento 2 theme.
## Important Steps
**1. Steps befeore getting statarted the theme development.**
- Activate developer mode.
- Give write permission in the `var` directory.
- Disable the caching system.

**2. Getting statarted the theme development.**
- Create the **vendor** directory of your theme.\
    `app/design/frontend/M2Theme`
- Create the **theme** directory of your theme.\
    `app/design/frontend/M2Theme/helloworld`
- Create the **theme declaration** file.\
    `app/design/frontend/M2Theme/helloworld/theme.xml`
- Create the **theme registration** file.\
    `app/design/frontend/M2Theme/helloworld/registration.php`
- Create the **static files directories**.\
    `app/design/frontend/M2Theme/helloworld/web`\
    `app/design/frontend/M2Theme/helloworld/web/css`\
    `app/design/frontend/M2Theme/helloworld/web/css/source`\
    `app/design/frontend/M2Theme/helloworld/web/fonts`\
    `app/design/frontend/M2Theme/helloworld/web/images`\
    `app/design/frontend/M2Theme/helloworld/web/js`
- Creating a **theme logo**.\
    Default logo name **logo.svg**.\
    Default directory `<theme_dir>/web/images/logo.svg`.\
    Simply put the file in the right directory.
- Creating a **theme logo with a different format**.\
    We will override `Magento_Theme` module.\
    `<theme_dir>/Magento_Theme/web/images/logo.png`\
    `<theme_dir>/Magento_Theme/layout/default.xml`
- Create a theme **preview image**.\
    `<theme_dir>/media/preview.jpg`
- Applying the theme.\
    Access the Magento admin panel.\
    Go to **Content->Design->Configuration**.\
    Select the **Hello World theme**.\
    Save the configuration.
## Magento UI Library 
- Evolution of the Magento System brought significant change to the way developers work.
- One of the technologies that have totally changed the way the development of themes for Magento 2 is understood: **The Magento User Interface Library**.
- The Magento User Interface Library is based on the LESS preprocessor, which facilitates the implementation of customizations in Magento 2 theme development.
- LESS technology as a CSS preprocessing solution promotes the writing of reusable and maintainable CSS codes.
- The Magento UI library is located in the `<magento_root>/lib/web/css/source/lib` directory.
### 1. LESS compilation in Magento 2
- **Server-Side compilation LESS**\
   Default compilation model used by the Magento 2 system.\
   Performed by the server using the LESS `PHP` library.\
   Suitable for production environments.   
- **Client-Side compilation LESS**\
   Performed by the client machine via the browser using the native `less.js` library.\
   Suitable for non-production environments.
### 2. Customizations using the Magento UI library
- **The _styles.less file**\
    Used as a standard nomenclature within the Magento 2 development environment.\
    Responsible for loading the Magento UI library to your project.
- **The _theme.less file**\
    Override the predefined custom variables.\
    Every variable that is rewritten in this file will be used throughout the Magento UI library on your theme.\
    There is no need to write new, complex CSS rules.



    