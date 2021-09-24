# V-Tabs: Shadom DOM Tabs Element

this is a tab element you can use as `<v-tabs>` in your markup. it's goal is to be a "render controller" navigation for a page. and to contain
a semantic HTML structure internally. i call it v-tabs as in vanilla javascript !

functionally it ties together a nav, a list, and some sections of markup which pop out of the shadow DOM when the slot name
and it's data attribute agree.

## use case :

if your just creating a simple static page, you can probably get away with some inline js and css for show and hiding from the DOM. This component
"renders" content to a slot, so as to keep that markup unparsed at all until it is navigated to, useful for embedding more components on a page although 
probably overkill for other purposes. 

my use for it is on static pages which feature dynamic components that need a high level nav for the content. in the case of my devlog, it toggles render of 
a "rolling blog" component and a "feed" component, giving my static page (full of static links) a lightning fast load time and snappy SPA feel. 
