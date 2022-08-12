# Vazir-Code-Font
A Persian (Farsi) Monospaced Font

## توسعه این پروژه متوقف و بایگانی شده است. این موضوع شامل تمامی ابعاد پروژه از طراحی گرفته تا رفع اشکال می‌شود.

<p dir="rtl">
فونت فارسی وزیرکد از نوع Monospaced یا تک‌فاصله 
ترکیب شده با فونت‌های Inconsolata و Hack
<br />

<a href="http://rastikerdar.github.io/vazir-code-font/">نمایش فونت</a> <br />
<a href="https://github.com/rastikerdar/vazir-code-font/releases">صفحه دریافت (دانلود) بسته فونت شامل فایل‌های ttf,woff,eot</a> <br />

با تشکر از برنامه <a href="https://fontforge.github.io">FontForge</a><br />

بر مبنای <a href="http://rastikerdar.github.io/vazir-font/">فونت وزیر</a>

</p>


<h1 dir="rtl">
طریقه استفاده در صفحات وب:
</h1>

<p dir="rtl">
کد زیر را در قسمت style یا فایل css وارد نمایید:
</p>


```css
@font-face {
  font-family: Vazir Code;
  src: url('Vazir-Code.eot');
  src: url('Vazir-Code.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Code.woff') format('woff'),
       url('Vazir-Code.ttf') format('truetype');
  font-weight: normal;
}

@font-face {
  font-family: Vazir Code Hack;
  src: url('Vazir-Code-Hack.eot');
  src: url('Vazir-Code-Hack.eot?#iefix') format('embedded-opentype'),
       url('Vazir-Code-Hack.woff') format('woff'),
       url('Vazir-Code-Hack.ttf') format('truetype');
  font-weight: normal;
}

pre, code {
  font-family: 'Vazir Code', 'Vazir Code Hack', monospaced;
}
```

## Install

#### Download
Grab the [latest release](https://github.com/rastikerdar/vazir-code-font/releases/latest) file.


#### CDN
Link fonts from the [RawGit](https://rawgit.com) CDN:

```html
<link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazir-code-font@v1.1.2/dist/font-face.css" rel="stylesheet" type="text/css" />
```

and integrate the font into your CSS:

```
font-family: 'Vazir Code', monospaced;
```

#### Homebrew
You can install the font on macOS machines by tapping the caskroom/fonts repo:  

```shell
brew tap caskroom/fonts
brew install font-vazir-code
```

#### NixOS
It can be also installed in NixOS:  

```nix
{
  enableDefaultFonts = true;
  fonts = with pkgs; [
    vazir-code-font
    ];
  fontconfig = {
    defaultFonts = {
      monospace = [ "Vazir Code"];
    };
  };
}
```

#### Arch Linux

Arch user's could use [vazir-code-fonts](https://aur.archlinux.org/packages/vazir-code-fonts/) package from [AUR](https://aur.archlinux.org/) repository to install vazir-code font. Use your favourite [AUR helper](https://wiki.archlinux.org/index.php/AUR_helpers) like pacaur or yaourt for installing package:

```shell
pacaur -S vazir-code-fonts
```


#### GNU/Linux
gnu/linux users could use [kateb](https://github.com/kiamazi/kateb) font manager, to install vazir-code font.

```
kateb install vazircode
or
kateb update vazircode
```
