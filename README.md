# Hugo site

Testing out how this works.
Been a while since I played with SSGs. 

## About Hugo

For when I inevitably forget...

### Directory structure

#### archetypes

contains templates for new content.
This is what gets used when you run `hugo new content posts/my-first-post.md`. 

#### assets 

contains global resources "usually passed through an asset pipeline."(?)
Anyway, things like images, CSS, and JS go here. 

#### config

config about the site. 
If this site stays simple, then the single `hugo.toml` in the root will suffice.

#### content

contains the Markdown files for the _content_ of the site. 

#### data

files like JSON, TOML, XLM go here.
These might augment content, config, localization, or navigation. 

#### i18n

internationalization.
Contains translation tables for multilingual sites.

#### layouts

contains templates to transform content, data, and resources into a complete website. 
These seem like the meat of where the templating goes. 

#### public

Shouldn't be here.
But it's what hugo generates when it builds the site. 

#### resources 

generated by Hugo. 
contains cached output from Hugo’s asset pipelines, generated when you run the hugo or hugo server commands.

Oh, that's what an "asset pipeline" is. 

#### static

contains files that will be copied directly into the public dir on build. 
Things like favicon, robots.txt, etc go here. 

Should _not_ be used for images, CSS, or JS. 
That method of using Hugo was deprecated with the introduction of "page bundles" and "asset pipelines".

#### themes

contains one or more themes, each in is own subdir. 
