# athena-document

As part of Athena I want to be able to use Markdown directly on my publications without having to render it serverside and without overhead for content creators. 

Usin the Polymer Philosophy of making everything a component, I've created athena-document to act as a host for Markdown content. This way we can style Markdown without affecting the host content. 


## Markdown Alternatives

There are 3 different markdown components that look promising

### marked-element

[marked-element](https://github.com/Polymer/marked-element) was created asa part of the Polymer elements and was the first markdown parsing element that I saw. It looks promising except for one thing: I haven't figured out how to use highlight.js with it. This renders the tool less than ideal for the kind of writing I want to do.

This is part of Polymer as a "molecule" (the collection that wraps libraries not part of the Polymer project

### re-markable

[re-markable](https://github.com/aktowns/polymer-re-markable) also wraps around the marked library. It has the same issue that `marked-element` does.

### juicy-markdown

[juicy-markdown](https://github.com/Juicy/juicy-markdown) presents the best selection of markdown elements. It allows you to use Github Flavored Markdown but it forces you to use the download of a scrapped version of the Github CSS file. This doesn't always work. 

It's not the end of the world. You can ignore Github's CSS and create your own. I've just gotten used to the way my markdown looks when stored in Github so using their CSS made sense to me.

### Others

[webcomponents.info](http://webcomponents.info/) has a selection of Markdown viewer and editor components. re-markable and juicy-markdown were selected from that list. 

### Common Mark

In an ideal world I'd get a library supporting Common Mark (Common Markdown) a new revision of 
the Markdown spec that fixes the inconsistencies across implementations. This effort has the backing of some of the largest Markdown users (Github, Stack Overflow, others) so it should finally allowusers  to write once and have it look the same everywhere. 
