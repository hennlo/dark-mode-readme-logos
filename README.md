# dark-mode-readme-logos
How to swap logos in README when using light or dark-mode 

Basically there are two appraoches:
1. [Using GitHub Markdown shortcuts](#Using-GitHub-Markdown-shortcuts)
2. [Using plain HTML code](#Using-HTML-code)

## Using GitHub Markdown shortcuts
**Pros**:
* Simple to embedd using github shortcuts
**Cons**:
* No image modification like resize possible
```markdown
![GitHub-Mark-Light](https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png#gh-light-mode-only)![GitHub-Mark-Dark](https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png#gh-dark-mode-only)
```
![GitHub-Mark-Light](https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png#gh-light-mode-only)![GitHub-Mark-Dark](https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png#gh-dark-mode-only)


## Using HTML code

```html
<picture>
  <source 
    srcset="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png" 
    media="(prefers-color-scheme: dark)">
  <a href="https://polypheny.org/">
    <img align="center" width="250" height="250" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png">
   </a>
</picture>
```


<picture>
  <source 
    srcset="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.pngogo-transparent.png" 
    media="(prefers-color-scheme: dark)">
  <img align="center" width="250" height="250" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png">
</picture>



