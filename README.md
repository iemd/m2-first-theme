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
    We will override `Magento_Theme` module.
    `<theme_dir>/Magento_Theme/web/images/logo.png`\
    `<theme_dir>/Magento_Theme/layout/default.xml`
- Create a theme **preview image**.\
    `<theme_dir>/media/preview.jpg`
- Applying the theme.\
    Access the Magento admin panel.\
    Go to **Store->Configuration->Design**.\
    Select the **Hello World theme**.\
    Save the configuration.