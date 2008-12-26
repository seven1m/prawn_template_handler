PrawnTemplateHandler
====================

Uber simple template handler for Prawn PDF views.

Installation
------------

    script/plugin install git://github.com/seven1m/prawn_template_handler.git

Usage
-----

In show.pdf.prawn:

    pdf.move_down 200
    pdf.text 'Hello World'

If you need to specify document options, add a @pdf line to your show method (optional):

    def show
      @pdf = Prawn::Document.new(:page_layout => :landscape)
    end

License
-------

Released into the Public Domain.
