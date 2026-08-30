# GEL highlighting support for kate
Adds support for syntax highlighting for the Genius Extension Language (.gel) language on kate. 

Has basic support for almost all built in functions, and commands. I didn't go much farther then that however, and Syntax highlighting for variables and functions is left out of this current version. I also left out highlighting for plotting commands, mainly because they have issues when running in kate's built in runtime.

<img width="254" height="276" alt="Screenshot_20260830_134145" src="https://github.com/user-attachments/assets/3a9b336e-14fc-4f8b-a88c-a5e9233d9c7e" />

| Links | Link info | 
| :---: | :---: |
| [Chapter 11 of Genius](https://www.jirka.org/genius-documentation/ch11.html) | Uses the "List of GEL functions" page on the jirka website page for genius's documentation.   |  
| https://www.jirka.org/genius-documentation/index.html | The genius manual |
| https://www.jirka.org/genius.html | Genius webpage |
| [Working with Syntax Highlighting](https://docs.kde.org/stable_kf6/en/kate/katepart/highlight.html) | The document page with info about Syntax highlighting in kate for developers |
| [Kate](https://apps.kde.org/kate/) | Link to the original kate text editor |

Using the highlighting 
---
First download the `gel.xml` file from the repo, or clone the repo with :

```
git clone https://github.com/KArLl0/GEL-highlighting-support-for-kate.git
```

With the xml downloaded, you'll need to find your data directory for kate's syntax highlighting

Use this guide to find where you'll need to put the `gel.xml` file.
| Install type | Install location|
|:---:|:---:|
| For local user	| $HOME/.local/share/org.kde.syntax-highlighting/syntax/
| For all users	| /usr/share/org.kde.syntax-highlighting/syntax/
| For Flatpak packages | 	$HOME/.var/app/flatpak-package-name/data/org.kde.syntax-highlighting/syntax/
| For Snap packages	| $HOME/snap/snap-package-name/current/.local/share/org.kde.syntax-highlighting/syntax/
| On Windows |	%USERPROFILE%\AppData\Local\org.kde.syntax-highlighting\syntax
| On macOS |	$HOME/Library/Application Support/org.kde.syntax-highlighting/syntax/

<sub>This table was gotten from the Working with Syntax Highlighting page on Kate's developer documentation.</sub>

You may need to create the `syntax/` folder, as modifying the `syntax-bundled/` is not ideal.

After, check by creating a gel file, and opening it with kate. Check Tools > Highlighting > Sources > GEL and select GEL, then check if functions are highlighted correctly.

Modifying 
---
If you wish to modify, I'd recommend looking into the [Working with Syntax Highlighting](https://docs.kde.org/stable_kf6/en/kate/katepart/highlight.html) page on kate's developer documentation. 

---
I do not have much experience with XML, so any enhancements will be an amazing help. 

Please support [KDE's Kate advance text editor]((https://apps.kde.org/kate/)), and [Genius Mathematics Tool and the GEL Language](https://www.jirka.org/genius.html)
