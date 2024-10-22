# Notice 📢
This theme is no longer supported. The problem is Vue3 would not work and Vue2 is deprecated.
If you still want a blogger theme that works, try [OP Blogger Theme](https://github.com/opdev1004/op-blogger-themes).
I am not going to use any web app frameworks like vue or react for future blogger theme development.


# Vuetilog 🥇

Blogger Theme built with Vue and Vuetify

## Other language:

[한국어](/lang/ko)

## Notice 📢

### Releasing version 0.1.8

- Fixed 'Reply' button. And this causes blog theme design changes, because theme needs to place blog post widget as it is provided from blogger system. Please have a look at `Editing Blog Widget in layout page from v0.1.8` bottom of this document.

### Releasing version 0.1.7

- Adding 18px bottom margin to heading tags. h1-h6.

### Releasing version 0.1.6

- Changing comments title element's color variable to body.font.color from sidebar.font.color

### Releasing version 0.1.5

- Added close button for closing sidebar for non-desktop view

## Example 📖

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

### Editing Blog Widget in layout page from v0.1.8

Some of section and widget would not show in layout page. Because Blogger's system cannot parse Vue and Vuetify's syntax. There are 2 ways to edit blog post widget. And you probably only need to do this once after install this theme for customization.

1. Move `Blog Widget` script to other Section (Somewhere like `Components` Section) from HTML Edit from Theme page. If you use wrapping arrow on the left side line number bar of HTML edit, you can easily copy and paste block of tag. Then you can edit `Blog Widget` from your layout page. Once you are done, you can copy that back to where it was.

```
<b:section class='Blog' id='Blog' name='Blog' showaddelement='no'>
<b:widget id='Blog1' locked='true' title='Blog Posts' type='Blog' version='2' visible='true'>
... more code
</b:widget>
</b:section>
```

2. Edit manually from HTML Edit. I don't recommend this.

### How to use code style in the post

1. `<pre><code></code></pre>`

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
