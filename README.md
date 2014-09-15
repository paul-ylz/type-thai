# Type Thai
## A gist to mimic changing keyboard language input to Thai without having to do it in the browser.

This keymap should work accurately for Chrome and Safari browsers.  

Credit to [Scott Harvey](https://github.com/scottharvey) for actually making it work :)  

In this example, `#new_entry_thai` is the `input` element that will now translate keypress events to Thai characters.  


    class ThaiWords.Views.Form extends Backbone.View

      template: JST['entries/form']

      render: ->
        $(@el).html(@template())
        new TypeThai @$('#new_entry_thai')
        this
