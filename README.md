### Template Brief (2019)

This describes the requirements for a simple, basic HTML template with a minimal amount of CSS, as light as possible, with a focus on reading text, and readability.

##### Version 1

1. *Targets modern browsers only;* Chrome, Firefox and Safari, both desktop and mobile, plus supported Microsoft browsers, which is currently IE 11 and Edge. No workarounds for older, unsupported browsers such as IE 9 and earlier are required, and baseline support for the few platforms that still support IE 10, such as certain versions of Windows Server, will be achieved by just keeping things simple, and letting it fail gracefully where necessary.

1. *No framework dependencies,* unless benefit can be clearly demonstrated vs. increased size and complexity. As in, no SASS, Less, Bootstrap, etc. This is clean HTML, with fresh, minimal CSS, and a minimal amount of Javascript. Must work when Javascript is disabled in the browser. The goal is to create a template that will last with a minimum amount of maintenance.

1. *No third-party dependencies;* needs to be completely self-contained. All resources necessary for the display of the page are loaded from the same domain, using relative links that work regardless of whether a page is placed in the root of a domain, or in a subdirectory under it.

1. *No custom fonts;* uses only standard system fonts, with a focus on readability. It is possible that custom fonts will be added later, such as for accessibility reasons (dyslexia, for example), but default system fonts must always provide the baseline.

1. *Fully responsive layout;* provides maximum readability for desktop, including large screens and older non-Retina screens, tablet, and mobile phones. Tablet will be mostly optimised for iPads, mobile will be tested with both iOS and Android devices, with an iPhone 5S as the baseline device in terms of size. Testing for various devices can be done in-house, as we have a set of devices available specifically for this purpose.

1. *Single column;* initial version will have a single column layout for all expected screen sizes, from large desktop to smallest targeted mobile. Optimised for readability, which probably means different `@media` stanzas for each device class, with differing font sizes, for example. Overall layout will have a maximum width that maintains readability even on large screens with a maximised browser window, and the column will be centered, but left-aligned for the text and other content.

1. *Header and footer;* header will have room for a centered square logo, and a navigation bar for up to three (3) items. The three items should be on one line for the desktop and tablet sizes, and can be on three lines for mobile. Footer will have its own font sizes and colours, but be otherwise as simple as possible, and its content will be left-aligned, like the main content area. Both header and footer will adhere to the same maximum width as the main content area.

1. *No inline CSS, or Javascript;* template will be used on systems with a strict [Content Security Policy](https://developer.mozilla.org/en-US/docs/Web/HTTP/CSP), and must not contain any inline CSS or Javascript. 
