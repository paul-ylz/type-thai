# Type Thai
## A gist to mimic changing keyboard language input to Thai without having to do it in the OS.

Developed for use [Thai Words](https://github.com/paul-ylz/thai_words)  

This keymap should work accurately for Chrome and Safari browsers only.  

Credit to [Scott Harvey](https://github.com/scottharvey) for heaps of coaching and actually getting the code to work in a tidy and organized way.  

In this example, `#new_entry_thai` is the `input` element that will translate keypress events to Thai characters.  


    class ThaiWords.Views.Form extends Backbone.View

      template: JST['entries/form']

      render: ->
        $(@el).html(@template())
        new TypeThai @$('#new_entry_thai')
        this

## Dependencies
- jQuery
- Coffeescript
