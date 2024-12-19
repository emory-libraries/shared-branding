In in-house Rails apps, the html.erb files are usually in app/views/shared.
If we are overriding another site or system (such as hyrax for the Open Emory site), the file may have to be renamed accordingly.

Common files include:
.scss files (can be compiled into a minified css internally by a rails gem or externally if necessary).
  fonts
  colors
  footer styles
Header
  The variations in the headers and the way they are built mean that currently the headers are made up of multiple files. 
  The central header file, if there is one, can render the navbar; utility links; logo; a search bar; a reusable, conditional announcement banner;
Footer
  The footer (_footer.html.erb) and the associated css file (_footer.scss), should be able to easily be dropped into a project with minimal adjustments or customizations.
  Add _footer.html.erb to the app/views/shared folder, and it will be referenced by something like <%= render partial: 'shared/footer' %> . 
