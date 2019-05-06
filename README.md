### Template Brief (2019)

This describes the requirements for a simple, basic HTML template with a minimal amount of CSS, as light as possible, with a focus on reading text, and readability.

##### Version 1

1. *Targets modern browsers only;* Chrome, Firefox and Safari, both desktop and mobile, plus supported Microsoft browsers, which is currently IE 11 and Edge. No workarounds for older, unsupported browsers such as IE 9 and earlier are required, and baseline support for the few platforms that still support IE 10, such as certain versions of Windows Server, will be achieved by just keeping things simple, and letting it fail gracefully where necessary.

1. *No framework dependencies,* unless benefit can be clearly demonstrated vs. increased size and complexity. As in, no SASS, Less, Bootstrap, etc. This is clean HTML, with fresh, minimal CSS, and a minimal amount of Javascript. Must work when Javascript is disabled in the browser. The goal is to create a template that will last with a minimum amount of maintenance.

1. *No third-party dependencies;* needs to be completely self-contained. All resources necessary for the display of the page are loaded from the same domain.

1. *No custom fonts;* uses only standard system fonts, with a focus on readability.
