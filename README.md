# Bootstrap4.0_concepts
Bootstrap related stuffs


Cards(Bootstrap 4)
Bootstrap’s cards provide a flexible and extensible content container with multiple variants and options.

About
A card is a flexible and extensible content container. It includes options for headers and footers, a wide variety of content, contextual background colors, and powerful display options. If you’re familiar with Bootstrap 3, cards replace our old panels, wells, and thumbnails. Similar functionality to those components is available as modifier classes for cards.

uiGradients - Beautiful colored gradients

https://uigradients.com
A handpicked collection of beautiful color gradients for designers and developers.

https://www.bootstrapcdn.com/

https://getbootstrap.com/docs/4.3/components/card/

//color
https://flatuicolors.com/palette/defo

// free images 
https://www.pexels.com/search/landscape/


Modal
Use Bootstrap’s JavaScript modal plugin to add dialogs to your site for lightboxes, user notifications, or completely custom content.

How it works
Before getting started with Bootstrap’s modal component, be sure to read the following as our menu options have recently changed.

Modals are built with HTML, CSS, and JavaScript. They’re positioned over everything else in the document and remove scroll from the <body> so that modal content scrolls instead.
Clicking on the modal “backdrop” will automatically close the modal.
Bootstrap only supports one modal window at a time. Nested modals aren’t supported as we believe them to be poor user experiences.
Modals use position: fixed, which can sometimes be a bit particular about its rendering. Whenever possible, place your modal HTML in a top-level position to avoid potential interference from other elements. You’ll likely run into issues when nesting a .modal within another fixed element.
Once again, due to position: fixed, there are some caveats with using modals on mobile devices. See our browser support docs for details.
Due to how HTML5 defines its semantics, the autofocus HTML attribute has no effect in Bootstrap modals. To achieve the same effect, use some custom JavaScript:
Copy
$('#myModal').on('shown.bs.modal', function () {
  $('#myInput').trigger('focus')
})