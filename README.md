# typst-tumthesis
This is a [typst](https://typst.app/) thesis template with front matter for TUM [informatics](https://www.cit.tum.de/cit/studium/studierende/abschlussarbeit-abschluss/informatik/#c4295) and TUM+LMU [bioinformatics](https://www.cit.tum.de/cit/studium/studiengaenge/master-bioinformatik/abschlussarbeit/#c2494). Therefore, it generally supports English and German as main document languages. It comes with ready-to-use outlines, configurable page numbers adapting to front and back matter, as well as flexible headers that can imitate `scrbook`. I also implemented `sidecap` and a basic `wrapfig` equivalent. 

Particular thanks to [zagoli](https://github.com/zagoli/simple-typst-thesis), [yangwenbo99](https://github.com/yangwenbo99/typst-uwthesis), [RubixDev](https://github.com/RubixDev/typst-outrageous/tree/main), [tingerrr](https://github.com/tingerrr/anti-matter), [lvignoli](https://github.com/lvignoli/typst-action) and [laurmaedje](https://github.com/typst/typst/issues/1295#issuecomment-1853762154)!


---

The TUM informatics and bioinformatics cover pages:
![tum cover pages](images/screen_00.png)

Table of contents with numbering up to level 2 headings, well-aligned fill characters and roman page numbers for the appendix: 

![a dummy table of contents](images/screen_01.png)

![overkill header and wrap figure](images/screen_03.png "an overkill left-hand page header and a wrapfig")


![example header and caption](images/screen_02.png  "right-hand page header with section info")


Defining a figure title for the list-of-figures is now less hacky:
```rs
#figure(
  image("/images/dingos.jpg", width: 100%),
  caption: flex-caption(
    [Another example full-width image], 
    [. Consumers are generally unaware that ...]),
) <dingos>
``````

![list of figures](images/screen_04.png)