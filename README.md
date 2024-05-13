# Semblance

Possible names:

-   Demeanor
-   Semblance
-   Facsimile
-   Mirage
-   Likeness
-   Sillhouette

Generates simulacrum plates using HTML and CSS using [html2canvas](https://html2canvas.hertzen.com/). Part of AUTOMATON, the simulacrum automation package.

-   [ ] https://gist.github.com/ricardoleme/8a4578493cf345d3fea381c796007f08

## How to

1.  get a book file. a book file is a json file in the following format:

        author: string;
        title: string;
        code: string;
        pages: Array<Page>;

    where a page is

        number: string;
        content: Array<string>;

1.  set background and text color in `src/style.css`
    -   https://color.adobe.com/create/image-gradient
    -   https://color.adobe.com/create/image
    -   https://cssgradient.io/
1.  `npm run dev` to start the server and then open the browser
1.  upload the file using the interface.
1.  use `page up` and `page down` to scan resulting images. edit parameters as needed
1.  if everything is ok, press `compile` and wait for it to process all images.
1.  press `download all`
1.  if you want to use it again, reload the page

## TODO

-   notification when all pages are compiled
-   convert md to html
-   number on counters is slightly wrong
-   having more than 6 plates per pages breaks it
-   check if no plate content is over limit. say what is the biggest one

##

-   fg

          --c1: rgb(55, 38, 44);
          --c2: linear-gradient(
              180deg,
              rgb(242, 208, 167),
              rgb(242, 208, 167),
              rgb(155, 149, 191)
          );
