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



<span id="mylogo">
<style>
#mylogo .darktheme,
#mylogo .lighttheme {
 display: none;
}

[data-theme="dark"] #mylogo .darktheme {
  display: inline;
}

[data-theme="light"] #mylogo .lighttheme {
  display: inline;
} 
</style>
<a href="https://polypheny.org/">
    <div>
    <img class="darktheme" align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-transparent.png#gh-light-mode-only" alt="Resume application project app icon">
     </div>
    <div>
    <img class="lighttheme" align="center" width="200" height="200" src="https://raw.githubusercontent.com/polypheny/Admin/master/Logo/logo-white-text.png#gh-dark-mode-only" alt="Resume application project app icon">
    </div>
</a>
</span>
