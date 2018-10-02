# Programming Fundamentals Book

Download and install AsciidocFX http://asciidocfx.com/

Fx is the main editor. The book is broken into chapters which are each their own .adoc file. There is also a book.adoc which contains the title page and includes all of the chapters. There is a preview page on the right side of the screen which is useful but does not render exactly the same as it will in the browser so take it with a grain of salt.

FX is great for editing but does not work with the code formatting we used to get line numbers in the examples. In order to build the html file with the correct formatting we need to use asciidoctor http://asciidoctor.org/ and the pygments code highlighting library. Instructions for how to install both of these are in the asciidoctor user manual http://asciidoctor.org/docs/user-manual/. They are both ruby gems so you'll need to install ruby as well if you don't have it https://www.ruby-lang.org/en/.

Once everything is installed you can build the html. Open up the command line terminal and navigate to the folder containing book.adoc. Run the command “asciidoctor –d book book.adoc” which will build the book.html file. You can do all of your editing in the individual chapterX.adoc files and as long as they are saved you only need to run that one command in the terminal.
Once the html file is built simply open it up in a browser to see the finished product.

To compile:

asciidoctor -d book book.adoc
