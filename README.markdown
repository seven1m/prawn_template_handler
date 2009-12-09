prawn_template_handler
======================

This is a template handler for Prawn PDF views in Rails. Simpler than Prawnto.

Installation
------------

    script/plugin install git://github.com/seven1m/prawn_template_handler.git

Usage
-----

The template registers the `pdf` mimetype, and the `prawn` template extension.

In the view file `show.pdf.prawn`:

    pdf.move_down 200
    pdf.text 'Hello World'
    
That's it!

If you need to specify document options, add a @pdf line to your show method, like so:

    def show
      @pdf = Prawn::Document.new(:page_layout => :landscape)
    end

License
-------

Released into the Public Domain.
