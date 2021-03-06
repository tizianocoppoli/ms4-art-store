<h1 align="center">Painters Canvas Shop</h1>

[View the live project here](https://ms4-art-store.herokuapp.com/)

This is the Painters Canvas Shop. In this ecommerce the user can find and buy different cavas with the most famous paintings in the world. It is designed to be responsible and accessible on multiple devices, making it easy to navigate for users on every device.

<h2 align="center"><img src="doc/website-home.png"></h2>

## User Experience (UX)

### Project Goals

The site's primary goal is to sell canvas to the visitors who are looking for something to decorate their home, or make a gift to someone really passionate about art. The site has 3 target audience and an admin role:

- Guest users (first time visitors)
- Casual customers (people who buy something without registering)
- Registered customers (people who like the website and want to purchase more products)
- Admin (can manage the products and the categories)


### User stories

  - ### Guest User Goals

    1. As a Guest User, I want to find easily the products.
    2. As a Guest User, I want to browse all canvas and use the search function.
    3. As a Guest User, I want to explore the product page, check more info about the shop like deliveries, returns and details.
  

  - ### Casual Customer Goals

    1. As a Casual Customer, I want to add a product to the bag and continue to browse the categories.
    2. As a Casual Customer, I want to check the bag anytime and have a look about how much I'm spending.
    3. As a Casual Customer, I want to update or remove a product from the bag.
    4. As a Casual Customer, I want to go to the checkout and pay.
    5. As a Casual Customer, I want to receive notifications to know if everything works or not.
  

  - ### Registered Customer Goals

    1. As a Registered Customer, I want to save my profile info for the next purchase.
    2. As a Registered Customer, I want to check my previous purchases in my profile page.
    3. As a Registered Customer, I want to edit my profile info to keep my profile updated.

  - ### Admin Goals

    1. As an Admin, I want to manage the products and categories.
    2. As an Admin, I want to access to the administration panel.
  

### UX - Five Planes Method

#### 1. Strategy
  The primary goal is to sell canvas to the visitors who are looking for something to decorate their home, or make a gift to someone really passionate about art.
  
#### 2. Scope
  Everything should be easy to understand. There is a simple navigation bar on the top. The user should be able to register, sign in, browse the products, add a product to the bag, and go to the checkout.

#### 3. Structure
  There is a home page which all the details about the site, and the button to browse the products. There is product page with all the products and each has an individual page with its details, picture, price, description, and a button to add to the bag. From the bag the user can go the checkout page and made the purchase, edit the bag and update/remove products. The registered user can go to the profile page and update the personal information.

#### 4. Skeleton
  The site is made with django. There are differents custom django apps:
  - home
  - products
  - checkout
  - bag
  - profile

  Each app manage a specific function of the website. The templates are made with a base template that is used for the navbar and the footer. Each app has templates that extend the base template. Check the wireframes for more details.

#### 5. Surface
  The website has a simple design with a few elements. The predominant colors are gold/black/white and the font style is handwritten and serif. Check the design section for more details.

### Design

#### Colour Scheme

- The palette has been generated with [Coolors](https://coolors.co/)

<img src="doc/palette.png">

  - Black: #000000
  - Davys Grey: #555555
  - Slate Gray: #6c757d
  - Gold Metallic: #d4af37
  - White: #ffffff

#### Typography

- 'Lato' is the main font used throughout the whole website, with 'Sans Serif' as the fallback font in case for any reason the font isn't being imported into the site correctly.
- 'Playfair Display' is a serif font used for headings.
- 'Pacifico' is am handwritten font used for logo and names.

#### Imagery
- Imagery is important. The images are all high quality pictures, designed to be striking and catch the user's attention. It also has a modern, energetic aesthetic.

### Wireframes

- Home Page - Desktop Wireframe - [View](doc/home_desktop.pdf)
- Home Page - Tablet Wireframe - [View](doc/home_tablet.png)
- Home Page - Mobile Wireframe - [View](doc/home_mobile.png)
- Canvas Page - Desktop Wireframe - [View](doc/product_desktop.pdf)
- Canvas Page - Tablet Wireframe - [View](doc/product_tablet.png)
- Canvas Page - Mobile Wireframe - [View](doc/product_mobile.png)

## Features

- Responsive on all device sizes
- Interactive form controls
- Button hover animations
- Notification toasts
- Search bar
- Sorting products by name/rating/category/price
- Add a product to the bag
- Update/remove a product to the bag
- Save user's info during the checkout
- Stripe checkout
- Stripe webhooks
- User Sign In/Sign Up
- Edit user informations
- Profile page with the history of orders
- Default images for the product
- Admin panel to manage products and categories
- Gmail integration to send automatic emails

### Features Left to Implement

- User profile
- More filters to improve the search function

## Technologies Used

### Languages Used

- [HTML5](https://en.wikipedia.org/wiki/HTML5)
- [CSS3](https://en.wikipedia.org/wiki/Cascading_Style_Sheets)
- [JavaScript](https://en.wikipedia.org/wiki/JavaScript)
- [Python](https://en.wikipedia.org/wiki/Python_(programming_language))

### Frameworks, Libraries & Programs Used

**Front-End**
* [Bootstrap](https://getbootstrap.com/) 
* [Font-Awesome](https://fontawesome.com/)
* [Google Fonts](https://fonts.google.com/)
* [jQuery](https://jquery.com/)
* [Balsamiq](https://balsamiq.com/)
* [Paint.net](https://www.getpaint.net/)

**Back-end**
* [Django](https://www.djangoproject.com/) 
* [Stripe](https://stripe.com/)

**Deployment**
* [Heroku](https://dashboard.heroku.com/)
* [AWS](https://aws.amazon.com/)
* [Git](https://git-scm.com/)
* [Github](https://github.com/)
* [Gitpod](https://gitpod.io/)

## Testing

For testing the following credentials can be used:
- Username: admin
- Password: password
- Email: admin@email.com

Card payments:
- Card number: 4242 4242 4242 4242
- Zip & CCV must be filled out with any integers.

The W3C Markup Validator and W3C CSS Validator Services were used to validate every page of the project to ensure there were no syntax errors in the project.

- [W3C HTML Validator](https://validator.w3.org/)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input)
- [Esprima JS Validator](https://esprima.org)
- [PEP8 online](http://pep8online.com/)

The deployed site was tested with Lighthouse for performance evaluation.

- [Lighthouse](https://developers.google.com/web/tools/lighthouse) - [Results](doc/lighthouse.png)

### Testing User stories from User Experience (UX) Section

- #### Guest User Goals

  - As a Guest User, I want to find easily the products.
    1. Upon entering the site, users immediately wiew the callout button to browse all products.
    2. The website provide a great navbar always visible with links for the products page and the categories.

  - As a Guest User, I want to browse all canvas and use the search function.
    1. In the navbar the user can search a name of a paintings or an artist.
    2. In the products page the user can scroll to see all the products and return to the top easily.
    3. In the products page each canvas has the price, the rating and the artist's name.

  - As a Guest User, I want to explore the product page, check more info about the shop like deliveries, returns and details.
    1. Each canvas has its own page where the user can read the description of the painting, add to the bag, check the price, zoom the image.
    2. In the home page the user can scroll to the section below the callot to read more details about the canvas itself, the shippings, and the returns.

- #### Casual Customer Goals

  - As a Casual Customer, I want to add a product to the bag and continue to browse the categories.
    1. In the product detail page the user can add a product to the bag and choose the quantity.
    2. After adding a product to the bag the user remain on the product page to continue browse the other products.

  - As a Casual Customer, I want to check the bag anytime and have a have a look about how much I'm spending.
    1. There is the bag icon in the navbar that shows anytime how much the user is spending.

  - As a Casual Customer, I want to update or remove a product from the bag.
    1. The user can go to the bag page and can change quantity to a product or remove it from the bag.
  
  - As a Casual Customer, I want to go to the checkout and pay.
    1. From the bag the user can go the checkout page and finalize the purchase.
  
  - As a Casual Customer, I want to receive notifications to know if everything works or not.
    1. The website implements toasts for notifications that show up on the top right corner each time an action is performed by the user.

- #### Registered Customer Goals

  - As a Registered Customer, I want to save my profile info for the next purchase.
    1. In the checkout page the user can flag the option to save the personal information in the profile.

  - As a Registered Customer, I want to check my previous purchases in my profile page.
    1. In the profile page the user can check the previous purchases anytime
    2. The user can click on a particular order to check the details.

  - As a Registered Customer, I want to edit my profile info to keep my profile updated.
    1. The user can go to the profile page and edit the informations anytime.
    2. In the checkout page the user can edit the information and flag the option to save them to update the profile.

- #### Admin Goals

  - As an Admin, I want to manage the products.
    1. The admin can edit or delete every product from the products page.
    2. The admin can edit or delete a product also from the product detail page.

  - As an Admin, I want to access to the administration panel.
    1. The admin can access to the django administration panel and edit the products and the categories.

### Further Testing

- The Website was tested on Google Chrome, Firefox and Microsoft Edge.
- The website was viewed on a variety of devices such as Desktop, Laptop, iPhone7, iPhone 8 & iPhoneX, iPad.
- A large amount of testing was done to ensure that all pages were linking correctly.

### Solved Bugs

- The footer didn't look good in the profile page because a </div> was missing in the template, and the footer weren't inside the proper container-fluid div. 

- The search function didn't work with category names. Fixed with the following code in the all_products view:
```
queries = Q(name__icontains=query) | Q(description__icontains=query) | Q(category__name__icontains=query)
```

# Deployment

### Installation Prerequisites

To be able to run the project the following technologies need to be installed in your IDE environment.
- Python3
- Git 
- pip3

You will need to be signed up to the following services:
- [Heroku](https://signup.heroku.com/)
- [AWS](https://aws.amazon.com/)
- [Stripe](https://stripe.com/)

### Cloning on GitHub

1. Login to GitHub.com.
2. Open [this repository.](https://github.com/tizianocoppoli/ms4-art-store)
3. Click "Code" then under "Clone" copy the link with the HTTPS URL.  
4. Go to the terminal in your IDE environment. 
5. Change the working directory to where you want the clone to be saved by typing `cd` and the name of the directory.
6. Type `git clone` and paste the copied HTTPS URL.
7. After pressing enter the clone will be saved to your chosen directory.

### Local Deployment On Gitpod

1. After cloning repository on GitHub. Go to your chosen IDE environment and open the clone directory.
2. Install the libraries from the requirements.txt, in the terminal type - `pip3 install -r requirements.txt`.
3. Set your environment variables in your gitPod settings or in an env.py file.
4. If setting variables within an env file add this to the .gitignore file so your variables are not exposed 
when pushing to gitHub.
5. Your environment variables will need to be set as follows:
- os.environ["DEVELOPMENT"] = "True"
- os.environ["SECRET_KEY"] = "Your Secret key"
- os.environ["STRIPE_PUBLIC_KEY"] = "Your Stripe Public key"
- os.environ["STRIPE_SECRET_KEY"] = "Your Stripe Secret key"
- os.environ["STRIPE_WH_SECRET"] = "Your Stripe WH_Secret key"
6. Create the database from the models by typing in the terminal `python3 manage.py makemigrations`. Followed by
`python3 manage.py migrate`
7. Load the data fixtures by typing in the terminal: `python3 manage.py loaddata products`
8. Create a superuser so you can log in to the Django admin by typing in the terminal: `python3 manage.py createsuperuser`
9. The site can now be run locally by typing in the terminal `python3 manage.py runserver`

### Heroku Deployment

1. After logging in to Heroku, select "Create New App" Choose the region closest to you and select "Create app".
2. On the resources tab, to provision the database in the add on field search for and select "Heroku Postgres".
3. A pop up should appear and under "Plan name" use "Hobby Dev-Free" and select "Provision".
4. Go to your IDE and type `pip3 install dj_database_url` and `pip3 install psycopg2-binary` as these need to be 
installed to use Postgres. Also `pip install gunicorn` for the webserver.
5. To make sure Heroku installs all of the apps when deployed save the requirements by typing in the terminal
`pip3 freeze > requirements.txt`
6. Back on Heroku under settings, select "Reveal config vars" and copy the key from DATABASE_URL.
7. In the project folder on settings.py in the database setting, comment out the current database setting.
8. Replace with: 
```
DATABASES = {
    'default': dj_database_url.parse('<Enter the copied DATABASE_URL key here>')
}
```
9. Add the data to the postgres database by typing in the terminal `python3 manage.py makemigrations`. Followed by
`python3 manage.py migrate`
10. Load the data fixtures by typing in the terminal: `python3 manage.py loaddata products`
11. Create a superuser so you can log in to the Django admin by typing in the terminal: `python3 manage.py createsuperuser`
12. Return to database setting in settings.py and remove code added in step 8 and uncomment the previous database setting.
13. Create a Procfile and add `web: gunicorn vision_furniture.wsgi:application`
14. Login to Heroku through the cli `heroku login -i`
15. Temporarily disable collect static by typing `heroku config:set DISABLE_COLLECTSTATIC=1`
16. Add `vision-furniture.herokuapp.com, localhost' to ALLOWED_HOSTS in settings.py.
17. The app can now be deployed by typing in the terminal `heroku git:remote -a vision-furniture` and `git push heroku master`
18. On Heroku dashboard under "Deploy" set "Deployment method" to connect to Gitub. Under "Automatic Deplays" set 
"Enable automatic deploy" so the code is automatically deployed to Heroku and GitHub.

### Add Static Files to AWS

1. Go to AWS and find S3 under services and create a new bucket, selecting the region closest to you and 
allowing all public access.
2. Go to the new bucket and under properties tab, turn on static website hosting.
3. Under permissions tab the CORS configuration tab and enter the following:
```
[
  {
      "AllowedHeaders": [
          "Authorization"
      ],
      "AllowedMethods": [
          "GET"
      ],
      "AllowedOrigins": [
          "*"
      ],
      "ExposeHeaders": []
  }
]
```

4. Go to the bucket policy tab. And select "policy generator" so we can create a security policy for this bucket.
5. Add in the following:
- Policy type: S3 bucket policy 
- Effect: Allow
- Principal: `*`
- Action: GetObject
- Copy the ARN from the bucket policy tab. And paste it into the ARN box at the bottom.
- Click Add statement. Then generate policy.
6. Copy the policy into the bucket policy editor.
7. Add `/*` onto the end of the resource key. Click Save.
8. Go to access control list tab and set the list objects permission for everyone under the Public Access section.
9. Create a user to access the bucket by selecting IAM from the servies menu.
10. Select "Groups" and select "Create new group". Add in a new group name and click next, next again then "create new group"
11. Create a policy to access the bucket, by selecting "policies" then "create policy". Select JSON tab and import managed policy. Search for 
s3 and import "AmazonS3FullAccess".
12. Copy the bucket policy ARN from the bucket policy in s3 > permissions. Paste it into the JSON resource key on create policy twice 
giving the second paste a `/*` at the end. Select "review policy". Give the policy a name and description and create the policy.
13. Go to "groups", select the new group, select "attach policy", search for the newly created policy and attach it to the policy.
14. Go to "users", add user, create a user name, give them programmatic access and select next.
15. Add the new user to the group and select next to create user then download the .csv file.
17. Go to your IDE terminal type: `pip3 intsall boto3` and `pip3 intall django-storages` to install the packages 
to connect to django. Type: `pip3 freeze > requirements.txt` so they get installed on heroku when its deployed.
18. Add 'storages' to installed apps on the settings.py file. Add the following code to tell Django which bucket to 
communicate with:
```
if 'USE_AWS' in os.environ:
    # Bucket Config
    AWS_STORAGE_BUCKET_NAME = 'vision-furniture'
    AWS_S3_REGION_NAME = 'eu-west-2'
    AWS_ACCESS_KEY_ID = os.environ.get('AWS_ACCESS_KEY_ID')
    AWS_SECRET_ACCESS_KEY = os.environ.get('AWS_SECRET_ACCESS_KEY_ID')
    AWS_S3_CUSTOM_DOMAIN = f'{AWS_STORAGE_BUCKET_NAME}.s3.amazonaws.com'

    # Static and media files
    STATICFILES_STORAGE = 'custom_storages.StaticStorage'
    STATICFILES_LOCATION = 'static'
    DEFAULT_FILE_STORAGE = 'custom_storages.MediaStorage'
    MEDIAFILES_LOCATION = 'media'

    # Override static and media URLs in production
    STATIC_URL = f'https://{AWS_S3_CUSTOM_DOMAIN}/{STATICFILES_LOCATION}/'
    MEDIA_URL = f'https://{AWS_S3_CUSTOM_DOMAIN}/{MEDIAFILES_LOCATION}/'
```
19. On Heroku add the AWS keys from the .csv file to the config vars. Also add USE_AWS: True, so the that the setting file knows 
to use the AWS configuration when deploying to Heroku. Remove the COLLECTSTATIC variable.
20. Push all the changes to Github. Which will trigger an automatic deployment to Heroku.

## Credits

I used the Code Institute Boutique Ado Mini-Project by Chris Zielinski as the main basis of this project.

### Code

- [Bootstrap](https://getbootstrap.com/): CSS library used throughout the project mainly to style and to make the site responsive using the grid system.

### Content

- Paintings descriptions and images are taken from [this blog article](https://www.timeout.com/newyork/art/top-famous-paintings-in-art-history-ranked)
- The remaining content was written by the developer.
- Psychological properties of colours text in the README.md was found [here](http://www.colour-affects.co.uk/psychological-properties-of-colours)

### Media

- Icons: [Noun Project](https://thenounproject.com/)
- Pictures: [Photowall](https://www.photowall.com/)
- Editing is made by the developer.

### Acknowledgements

- My Mentor for continuous helpful feedback.
- Tutor support at Code Institute for their support.
