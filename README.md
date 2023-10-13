# Vuetilog

Blogger Theme built with Vue and Vuetify

## Other language:

[한국어](/lang/ko)

## Notice

### Releasing version 0.1.1

The design has been updated.

### Releasing version 0.1.0

The design has been updated. Popular posts and Featured post have been removed from vue components. You can use Popular posts and Featured posts from theme system instead. But you have to style them yourself.

## Example

[https://vuetilog.blogspot.com/](https://vuetilog.blogspot.com/)

## Download

[https://github.com/opdev1004/vuetilog/releases/](https://github.com/opdev1004/vuetilog/releases/)

## Features:

1. Development with Vue and Vuetify
2. Responsive Web design
3. SEO
4. Better label control

## Installation:

1. Apply Contempo theme to your blog.
2. Restore theme with vuetilog.xml or copy and paste vuetilog theme in HTML edit.
3. Edit any settings in your needs.

### How to use code style in the post

1. Select your code block in the editor by mouse dragging
2. Set them as normal instead of paragraph
3. Change to HTML view
4. Set class to the div element for your code with "code". eg. `class="code"`

### Layout System

| Section             | Description                                                                                                        |
| ------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Nav Top             | You can add any sidebar widgets here.                                                                              |
| Label Section       | You can only add labels.                                                                                           |
| Nav Bottom          | You can add any sidebar widgets here.                                                                              |
| Main Content Top    | You can add any main content widgets here. eg. ads                                                                 |
| Main Content Bottom | You can add any main content widgets here. eg. ads                                                                 |
| Components          | This is for the theme developers. Specially for the widgets that is going to be modified a lot as a vue component. |
| Bottom Section      | You can add any footer widgets here.                                                                               |

## Contribution

You are welcome to improve Vuetilog.
You can contribute by opening a pull request in this repository.

## Theme Development Details

### Theme load order

1. Blogger Template System Generates HTML file from vuetilog theme
2. Webbrowser loads the blog page
3. Loads Vue, Vuetify, CSS and many other things from the head tag
4. Go through id='init-wrapper' div tag where majority of elements that will be componentized later
5. Go through Vue App Template
6. Creates loading overlay with Vue from the top of body tag
7. Componentizes the elements from id='init-wrapper' div tag
8. Create Vue app with components and data
9. Removes init-wrapper div tag
10. Removes loading overlay

### How to use Vue and Vuetify?

As long as your tags are part of components and vue app template, they are going to be loaded.

### Vuetilog Components

| Components          | Location               | Description                                                |
| ------------------- | ---------------------- | ---------------------------------------------------------- |
| nav-top             | Left Navigation Drawer | This component is for any sidebar widgets.                 |
| label-section       | Left Navigation Drawer | This component is designed to contains only label widgets. |
| nav-bottom          | Left Navigation Drawer | This component is for any sidebar widgets.                 |
| main-content-top    | Main Page              | This component is for any widgets for main page. eg. ads   |
| main-content-bottom | Main Page              | This component is for any widgets for main page. eg. ads   |
| pagination          | Main Page              | This component is for placing pagination.                  |
| posts               | Main Page              | This component is for placing blog posts and pages.        |
| comments            | Main Page              | This component is for placing comments.                    |
| post-feeds          | Main Page              | This component is for placing post feeds link.             |
| bottom-section      | Main Page              | This component is designed for footer of blog.             |

### 👼 Become a Sponsor

- [Ko-fi](https://ko-fi.com/opdev1004)
- [Github sponsor page](https://github.com/sponsors/opdev1004)

### 🎁 Shop

- [RB Rino Shop](https://www.redbubble.com/shop/ap/149559711)
- [RB Geargom Shop](https://www.redbubble.com/people/Geargom/shop)

## 👨‍💻 Author

[Victor Chanil Park](https://github.com/opdev1004)

## 💯 License

MIT, See [LICENSE](./LICENSE).
