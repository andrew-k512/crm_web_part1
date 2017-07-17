
    Create a new directory called public at the root of your project.
    Create a file called styles.css in the public directory.
    Create a file called layout.erb in the views directory.

Our application should currently have at least three different views. Repeating the same header and footer code (etc) in all of these ERB files would not be very DRY. Layouts are the solution to code repetition across your HTML and are a common part of any templating language, not just Sinatra. We'll become acquainted with these again when we get to Rails.

Add a basic HTML page structure (with an <html>, <head>, and <body>) in layout.erb (you should be able to make Atom do the work for you by typing html at the top of the empty file and then hitting enter). You should also add a <link> in your <head> to import your stylesheet, and a <%= yield %> inside the <body>.

Layouts use yield, which you may have never seen before. yield allows us to dynamically insert other views inside this file. The yield statement should be wherever you want the page-specific content to appear.
