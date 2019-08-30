# Huesristics / Checklists 
'''Heuristics and checklist are really bad for actually developing a culture of excellence. Read this article to get a perspective on this: [Accessibility Checcklists: Just say no](https://medium.com/@sheribyrnehaber/accessibility-checklists-just-say-no-c9a68c8f2c90)

BUT

They can be a good starting point. 
Part of the battle is to make sure you update them as you learn 

Please update me :-)
'''

There now follows a series of checlists that dive deeper and deeper into A11Y with a primary focus on Content developers.

## Main areas of disability 

### Visual
- Blind, Low vision, Colour blind...

### Speach
- Inability or difficulty speaking or being understood

### Hearing
- Deaf or hard of hearing

### Cognitive
- Dyslexia, ADD, Epilepsy, Autistic spectrum disorders...

### Motor
- Physically disabled people who might find it hard to type or use a mouse.


## How permanent these disabilities might be
They might be:
- **Permamnent**: Such as someone who has lost an arm
- **Temporary**: 	Such as someone who has broken an arm
- **Situational**: Such as someone who is holding a baby and does not have use of that arm for other tasks


## A Basic Checklist



## A more in depth checklist
- [ ] Make sure there is enough contrast between text and its background color [More Info](http://accessibility.voxmedia.com/#designers-1)
- [ ] Don't indicate important information using color alone [More Info](http://accessibility.voxmedia.com/#designers-2)
- [ ] Pair values of colors together (not only hues) to increase contrast [More Info](http://accessibility.voxmedia.com/#designers-3)
- [ ] Design focus states to help users navigate and understand where they are [More Info](http://accessibility.voxmedia.com/#designers-5)
- [ ] Help users understand inputs, and help them avoid and correct mistakes [More Info](http://accessibility.voxmedia.com/#designers-6)
- [ ] Write good alt text for your images [More Info](http://accessibility.voxmedia.com/#designers-7)
- [ ] Be as consistent and clear as possible in layout and copy [More Info](http://accessibility.voxmedia.com/#designers-9)
- [ ] Use the correct HTML element for your content [More Info](http://accessibility.voxmedia.com/#engineers-1)
- [ ] Support keyboard navigation [More Info](http://accessibility.voxmedia.com/#engineers-2)
- [ ] Understand and use HTML landmarks [More Info](http://accessibility.voxmedia.com/#engineers-3)
- [ ] Write good alt text for your images [More Info](http://accessibility.voxmedia.com/#engineers-4)
- [ ] Help users understand inputs, and help them avoid and correct mistakes [More Info](http://accessibility.voxmedia.com/#engineers-6)
- [ ] Use ARIA attributes when applicable [More Info](http://accessibility.voxmedia.com/#engineers-7)
- [ ] Give users a way to skip top level navigation to access main content [More Info](http://accessibility.voxmedia.com/#engineers-8)
- [ ] Make links descriptive [More Info](http://accessibility.voxmedia.com/#engineers-9)
- [ ] Avoid images and iconography in pseudo-elements [More Info](http://accessibility.voxmedia.com/#engineers-10)
- [ ] Make SVGs accessible to assistive technology [More Info](http://accessibility.voxmedia.com/#engineers-11)
- [ ] Hide decorative elements from screen readers [More Info](http://accessibility.voxmedia.com/#engineers-12)
- [ ] Create alternate routes for users to access information [More Info](http://accessibility.voxmedia.com/#engineers-13)
- [ ] Links should be visually identifiable and have clear :focus and :active states [More Info](http://accessibility.voxmedia.com/#engineers-14)
- [ ] Users should be able to navigate through content using their keyboard. [More Info](http://accessibility.voxmedia.com/#qa-2)
- [ ] Users should be able to navigate content using a screen reader. [More Info](http://accessibility.voxmedia.com/#qa-3)
- [ ] Decorative images should not be visible to screen readers. [More Info](http://accessibility.voxmedia.com/#qa-6)



## A WCAG refernced checklist


## Tools
- [ ] Use these tools to help make your work accessible [More Info](http://accessibility.voxmedia.com/#tools-1)
 - [WCAG 2.0 guidelines to review best practices](http://code.viget.com/interactive-wcag/#responsibility=design&level=aa),
 - [WAVE (Web Accessibility Evaluation Tool) Chrome Extension to check accessibility across your products](https://chrome.google.com/webstore/detail/wave-evaluation-tool/jbbplnpkjmmeebjpijfedlgcdilocofh?hl=en-US),
 - [Color Contrast Analyzer App to analyze color contrast](https://www.paciellogroup.com/resources/contrastanalyser/),
 - [Color Safe to make accessible color palettes](http://colorsafe.co/),
 - [Color Oracle to simulate color blindness](http://colororacle.org/index.html),
 - [Sim Daltonism to simulate color blindness](https://michelf.ca/projects/sim-daltonism/)

## References
[Justine Pocock's Github List](https://gist.github.com/justinepocock/533e0ae9d366b9629c27789d414156ed) Based on Voxmedia's list

[Voxmedia A11y checklist](http://accessibility.voxmedia.com)

## Test Area



<style>
.tablelines table, .tablelines td, .tablelines th {
        border: 1px solid black;
        margin: 5px
        }
</style>

| Level  | Area | Note  | Resources  | Comments |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |
{: .tablelines}






This is a growing list of accesibility hueristics  

## Content
Content is the most important part of your site.

 - Use plain language and avoid figures of speech, idioms, and complicated metaphors.
 - Make sure that button, a, and label element content is unique and descriptive.
 - Use left-aligned text for left-to-right languages, and right-aligned text for right-to-left languages.

## Global code
Global code is code that affects your entire website.

 - Validate your HTML.
 - Use a lang attribute on the html element.
 - Provide a unique title for each page or view.
 - Ensure that viewport zoom is not disabled.
 - Use landmark elements to indicate important content regions.
 - Ensure a linear content flow.
 - Avoid using the autofocus attribute.
 - Remove session timeouts.
 - Remove title attribute tooltips.

## Keyboard
It is important that your interface and content can be operated, and navigated by use of a keyboard. Some people cannot use a mouse, or may be using other assistive technologies that may not allow for "hovering" or precise clicking.

 - Make sure there is a visible focus style for interactive elements that are navigated to via keyboard input.
 - Check to see that keyboard focus order matches the visual layout.
 - Remove invisible focusable elements.
 
## Images
Images are a very common part of most websites. There are techniques you can use to help make sure they are enjoyable by all.

### All images
 - Make sure that all img elements have an alt attribute.
 - Make sure that decorative images have empty alt attribute values.
 - Provide a text alternative for complex images such as charts, graphs, and maps.
 - For images containing text, make sure the alt description includes the image's text.
 
### SVGs
SVGs are images described using markup.

 - Make sure that svg elements include the code focusable="false" when they are the child element of a focusable element.
 - Add aria-hidden="true" to svg that is decorative.
 - Make sure that svg utilizing the use element has whitespace between the svg and use elements.
 - Ensure that img elements with an svg source includes the role="img" attribute.

## Headings
Heading elements (h1, h2, h3, etc.) help break up the content of the page into related "chunks" of information.

 - Use heading elements to introduce content.
 - Use only one h1 element per page or view.
 - Heading elements should be written in a logical sequence.
 - Don't skip heading levels.

## Lists
Lists let people know the content is related, and how many items are included in the grouping.

 - Use list elements (ol, ul, and dl) for list content.

## Controls
Controls are interactive elements such as links and buttons that let a person navigate to a destination or perform an action.

 - Use the a element for links.
 - Ensure that links are recognizable.
 - Ensure that controls have :focus states.
 - Use the button element for buttons.
 - Provide a skip link and make sure that it is visible when focused.
 - Identify links that open in a new window.

## Tables
Tables are a structured set of data that help people understand the relationships between different types of information.

 - Use the table element to describe tabular data.
 - Use th for table headers (with appropriate scope attributes).
 - Use the caption element to provide a title for the table.

## Forms
Forms allow people to enter information into a site for processing and manipulation. This includes things like sending messages and placing orders.

 - All inputs in a form are associated with a corresponding label element.
 - Use fieldset and legend elements where appropriate.
 - Inputs use autocomplete where appropriate.
 - Make sure that form input errors are displayed in list above the form after submission.
 - Associate input error messaging with the input it corresponds to.
 - Make sure that error, warning, and success states are not visually communicated by just color.

## Media
Media includes content such as pre-recorded and live audio and video.
 - Make sure that media does not autoplay.
 - Ensure that media controls use appropriate markup.
 - Check to see that all media can be paused.
### Video
 - Confirm the presence of captions.
 - Remove seizure triggers.
### Audio
 - Confirm that transcripts are available.

## Appearance
How your site content looks in any given situation.

 - Check your content in specialized browsing modes.
 - Increase text size to 200%.
 - Double-check that good proximity between content is maintained.
 - Make sure color isn't the only way information is conveyed.
 - Use a simple, straightforward, and consistent layout.

## Animation
Content that moves, either on its own, or when triggered by a person activating a control.

 - Ensure animations are subtle and not do not flash too much.
 - Provide a mechanism to pause background video.
 - Make sure all animation obeys the prefers-reduced-motion media query.

## Color contrast
Color contrast is how legible colors are when placed next to, and on top of each other.

 - Check the contrast for all normal-sized text.
 - Check the contrast for all large-sized text.
 - Check the contrast for all icons.
 - Check the contrast of borders for input elements (text input, radio buttons, checkboxes, etc.).
 - Check text that overlaps images or video.
 - Check custom ::selection colors.

## Mobile/Touch
Things to check to best support different device form factors.

 - Check that the site can be rotated to any orientation.
 - Remove horizontal scrolling.
 - Button and link icons can be activated with ease.
 - Ensure sufficient space between clickable items in order to provide a scroll area.
