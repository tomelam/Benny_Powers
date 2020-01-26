# Codementor session with Benny Powers

## Background and Requirements

1. There is a lot about HTTP and HTML I don't know, including probably a lot
   of the basics.

1. I hope that our session will not take more than 30 minutes and that any
   minutes beyond that will be billed on a prorated basis, not in 15-minute
   increments.

1. I am writing a set of [BiwaScheme](https://www.biwascheme.org/) functions
   and macros to add web components to a page using
   [BiwaScheme's foreign function interface](https://www.biwascheme.org/doc/reference.html#js-interface).
   I want to *learn* what methods and event handlers to write so that a web app
   authored *on the fly* in BiwaScheme-in-the-browser will have all normal but
   basic capabilities. By *on the fly* I mean a whole web app will be created
   by BiwaScheme. The macro
   [define-event-handler](https://raw.githubusercontent.com/Mashweb/seq_webapp_biwascheme/master/mini-framework.scm)
   is my interface to
   [BiwaScheme's interface to JavaScript events](https://www.biwascheme.org/doc/reference.html#js-interface).
   
   By basic, I mean nonspecialized, nothing as complex as drag-and-drop or
   multimedia (at least not yet). Perhaps going through just the programmatic
   creation of a web component for a button would be enough for my *learning*.
   Hopefully even a nontechnical person should be able to understand the
   connections between the components and their actions. See
   [Mashweb.Club](http://mashweb.club/) and
   [my sequentially programmed web app](https://doc.mashweb.club/experiments/seq_webapp_biwascheme/). (Skip down to the Scheme code in the section
   'Try It Now'. I think you'll be able to read the code even if you never
   encountered Scheme before.)

1. I want to use web components from a good, well-known library or catalog,
   so I want to *learn* what libraries and catalogs would meet my needs.
   The library or catalog should support three or four of the standards
   that make up
   [web components v1](https://www.webcomponents.org/introduction) and should
   work with 99% of web agents (mainly browsers) that were up to date as far
   back as a few years ago (say, 3 to 5 years). I'm not sure whether I should
   want the components to support the HTML template standard.
   I don't mind using a polyfill if it is small and fast (slow-mobile-friendly).

   I want to avoid complications like BEM (Block Element Modifier) if such
   complications are unnecessary due to the evolution of the standards and the
   browsers. It appears that Material Components for the Web uses BEM.
   See, for example,
   [Button](https://material-components.github.io/material-components-web-catalog/#/component/button).

1. I want a simple but fully backward compatible button and other replacements
   for standard HTML elements so that I can standardize my design system
   and encapsulate my web components' styles. I want these replacements to be
   usable wherever standard HTML elements are usable. They should be just as
   nestable as standard HTML elements are. I want to *learn* which components
   of the selected libraries and catalogs will serve these purposes.

1. I believe that most elements, whether standard or custom, can take care of
   many or most of their own responses to events
   in the sense that no JavaScript is necessary to respond to such events
   as focus, blur, pagehide, animationstart, etc.
   See [MDN's event reference](https://developer.mozilla.org/en-US/docs/Web/Events#Standard_events).
   I want to *learn* whether I am correct or not about this assumption.

1. The types of data binding used by standard HTML elements should work with
   the web components: methods like *submit*, *keydown*, *keyup*, *keypress*,
   *click*, *mousedown*, *mouseup*, *mouseenter*, *mouseleave*, *mousemove*,
   *mouseover*, *touchend*, *touchmove*, *touchstart*, etc.
   Basically, at a minimum boring web apps should be supported.
   I want to *learn* the standard APIs necessary to author any boring web app. 
