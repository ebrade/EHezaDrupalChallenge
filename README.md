# EHeza Drupal Challenge


This project uses Drupal 8 and It runs in ddev containers.
# Getting Started with the starter code
Assuming the ddev is already installed.
1. Clone the starter repo
 - Clone or Fork this [drupal-starter repo](https://github.com/Gizra/drupal-starter)
 2. Run the following commands under Root Repo folder
 ```sh
ddev composer install
cp .ddev/config.local.yaml.example .ddev/config.local.yaml
ddev restart
 ```
 In case you have already installed above repo run
 ```sh
 ddev rm --unlist
 ```
# Installing the OG Module
Under project root run
```sh
$ ddev composer require drupal/og
$ ddev exec drush en og
```

# Accessing the Web Drupal Site
To connect to  the this Drupal website run 
```sh
ddev start
```
 Or Ignore above command If you have run the ddev restart command
The above command will give you one time authencation access link to reset the Admin username and password.

# configure a new content type as a Group.

1. Go to the Admin Pannel **clicks on extend** and go down to tick the Organic Groups and Organic Groups UI modules and click **Install** to enable them.
## Creating New content type as Group
- Under **Structure** clicks on **content types** and click add content
- Fill the new content generation form (Title, Description, Label) and in the Organic groups tick **Group**
## Creating Group content
- Under **Content** click **add content**
- Choose the name of the above created Group Content Type(eg. Group)
- Fill Title of content, description and other required configurations
- click save.

### Other parts of the challenge are not done.




