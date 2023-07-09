پروژه را به صورت زیر کلون کنید:

```bash
git clone --recurse-submodules https://github.com/mdpe-ir/dialect.git
```
و بعد با اجرای دستورات زیر ران بگیرید:

```bash
cd dialect
meson builddir --prefix=/usr/local
sudo ninja -C builddir install
meson builddir
meson configure builddir -Dprefix=$(pwd)/builddir/testdir
ninja -C builddir install
ninja -C builddir run
```



### نکات:
البته حواستون باشه این پکیجا حتما نصب باشه رو توزیع :

`tesseract-ocr`

`tesseract-ocr-all`

`imagemagick`

`gnome-screenshot`

### لیست انجام کار:
شاید یه لانچر براش زدم یه روزی 
ولی فعلا همین کار راه بندازه
