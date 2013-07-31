emdjs
=====

JS implementation of evermd in a more canonical way

See the post: <http://blog.hupili.net/p--20130731-markdown-extension/>

Original perl implementation of [evermd](https://github.com/hupili/evermd) is not flexible.
Fixing with a specific MD backend will drastically lower down the usability.
In the above post, I described the canonical way:

   * Use code block to protect your materials from being messed up by any compilers.
   * Use JS to re-render them as you wish.

I already have several polishing implementations on my blog.
In this project, I will turn the original perl implementation into a JS implementation.
This is a fully backward compatible extension with any standard backend.

Examples
--------

Inline formula:

    `$\frac{1}{e^x}$`

Block (display) formula:

    ```
    $$\frac{1}{e^x}$$
    ```
    
Block (display) formula2:

    `$$\frac{1}{e^x}$$`

Block (display) formula 3:

    ```formula
    \frac{1}{e^x}
    ```
    
Table:

    ```table
    & h1 & h2 & h3
    -----
    & c1 & c2 & c3
    && span2 & c4
    ```
    
Variable, current time:

    ```var
    now
    ```
    
variable, table of contents:

    ```var
    TOC
    ```

more examples to add... 
