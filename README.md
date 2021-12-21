# dark-mode-readme-logos
How to swap logos in README when using light or dark-mode 

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
<a href="https://polypheny.org/">
    <div>
    <img align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png#gh-light-mode-only" alt="Resume application project app icon">
     </div>
    <div>
    <img align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png#gh-dark-mode-only" alt="Resume application project app icon">
    </div>
</a>
```


<picture>
  <source 
    srcset="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png" 
    media="(prefers-color-scheme: dark)">
  <a href="https://polypheny.org/">
    <img src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png">
   </a>
</picture>

<!--
<a href="https://polypheny.org/">

    <img align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png#gh-light-mode-only" alt="Resume application project app icon">

    <img  align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png#gh-dark-mode-only" alt="Resume application project app icon">

</a>
-->

