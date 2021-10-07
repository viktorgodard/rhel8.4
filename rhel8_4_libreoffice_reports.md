20211006

Requirements for CLI based report generation of .xls,.word and .pdf docs using Libre Office headless
https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/install-campaign-on-prem/installing-campaign-in-linux-/prerequisites-of-campaign-installation-in-linux.html?lang=en

RHEL8.4

# LIBRARIES:

# yum search c-ares
# c-ares.x86_64 : A library that performs asynchronous DNS operations
c-ares.i686 : A library that performs asynchronous DNS operations

# rpm -qa |grep "c-ares"
# c-ares-1.13.0-5.el8.x86_64

# yum info c-ares.x86_64
Installed Packages
Name         : c-ares
Version      : 1.13.0
Release      : 5.el8
Architecture : x86_64
Size         : 222 k
Source       : c-ares-1.13.0-5.el8.src.rpm
Repository   : @System
From repo    : anaconda
Summary      : A library that performs asynchronous DNS operations
URL          : http://c-ares.haxx.se/
License      : MIT
Description  : c-ares is a C library that performs DNS requests and name resolves
             : asynchronously. c-ares is a fork of the library named 'ares', written
             : by Greg Hudson at MIT.


# FONTS:

# yum search xorg-x11-fonts-base xorg-x11-fonts-75dpi bitstream-vera-fonts dejavu-lgc-fonts
# xorg-x11-fonts-75dpi.noarch : A set of 75dpi resolution fonts for the X Window System      # <-- only one found

# yum info xorg-x11-fonts-75dpi.noarch
Available Packages
Name         : xorg-x11-fonts-75dpi
Version      : 7.5
Release      : 19.el8
Architecture : noarch
Size         : 2.8 M
Source       : xorg-x11-fonts-7.5-19.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : A set of 75dpi resolution fonts for the X Window System
URL          : http://www.x.org
License      : MIT and Lucida and Public Domain
Description  : A set of 75 dpi fonts used by the X window system.


# bitstream or vera fonts not found.
# x11 fonts base not found

# What other fonts are available?

# yum search fonts |grep x11
xorg-x11-fonts-100dpi.noarch : A set of 100dpi resolution fonts for the X Window System
# xorg-x11-fonts-75dpi.noarch : A set of 75dpi resolution fonts for the X Window System
xorg-x11-fonts-ISO8859-1-100dpi.noarch : A set of 100dpi ISO-8859-1 fonts for X
xorg-x11-fonts-ISO8859-1-75dpi.noarch : A set of 75dpi ISO-8859-1 fonts for X
xorg-x11-fonts-ISO8859-14-100dpi.noarch : ISO8859-14-100dpi fonts
xorg-x11-fonts-ISO8859-14-75dpi.noarch : ISO8859-14-75dpi fonts
xorg-x11-fonts-ISO8859-15-100dpi.noarch : ISO8859-15-100dpi fonts
xorg-x11-fonts-ISO8859-15-75dpi.noarch : ISO8859-15-75dpi fonts
xorg-x11-fonts-ISO8859-2-100dpi.noarch : A set of 100dpi Central European language fonts for X
xorg-x11-fonts-ISO8859-2-75dpi.noarch : A set of 75dpi Central European language fonts for X
xorg-x11-fonts-ISO8859-9-100dpi.noarch : ISO8859-9-100dpi fonts
xorg-x11-fonts-ISO8859-9-75dpi.noarch : ISO8859-9-75dpi fonts
xorg-x11-fonts-Type1.noarch : Type1 fonts provided by the X Window System
xorg-x11-fonts-misc.noarch : misc bitmap fonts for the X Window System

# yum search dejavu
=============================================== Name & Summary Matched: dejavu ================================================
bpg-dejavu-sans-fonts.noarch : DejaVu Sans with BPG Georgian changes
dejavu-fonts-common.noarch : Common files for the Dejavu font set
==================================================== Name Matched: dejavu =====================================================
# dejavu-lgc-sans-fonts.noarch : Variable-width sans-serif font faces, Latin-Greek-Cyrillic subset
# dejavu-sans-fonts.noarch : Variable-width sans-serif font faces
dejavu-sans-mono-fonts.noarch : Monospace sans-serif font faces
dejavu-serif-fonts.noarch : Variable-width serif font faces

# yum info dejavu-lgc-sans-fonts.noarch
Available Packages
Name         : dejavu-lgc-sans-fonts
Version      : 2.35
Release      : 7.el8
Architecture : noarch
Size         : 1.1 M
Source       : dejavu-fonts-2.35-7.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : Variable-width sans-serif font faces, Latin-Greek-Cyrillic subset
URL          : http://dejavu-fonts.org/
License      : Bitstream Vera and Public Domain
Description  : 
             : The DejaVu font set is based on the “Bitstream Vera” fonts, release 1.10. Its
             : purpose is to provide a wider range of characters, while maintaining the
             : original style, using an open collaborative development process.
             : 
             : This package consists of the DejaVu sans-serif variable-width font faces, with
             : unicode coverage restricted to Latin, Greek and Cyrillic.

# yum info dejavu-sans-fonts.noarch
Available Packages
Name         : dejavu-sans-fonts
Version      : 2.35
Release      : 7.el8
Architecture : noarch
Size         : 1.5 M
Source       : dejavu-fonts-2.35-7.el8.src.rpm
Repository   : rhel-8-baseos-rhui-rpms
Summary      : Variable-width sans-serif font faces
URL          : http://dejavu-fonts.org/
License      : Bitstream Vera and Public Domain
Description  : 
             : The DejaVu font set is based on the “Bitstream Vera” fonts, release 1.10. Its
             : purpose is to provide a wider range of characters, while maintaining the
             : original style, using an open collaborative development process.
             : 
             : This package consists of the DejaVu sans-serif variable-width font faces, in
             : their unabridged version.



# LIBRE OFFICE:

# yum search libreoffice-writer
# libreoffice-writer.x86_64 : LibreOffice Word Processor Application

# yum search libreoffice-calc
# libreoffice-calc.x86_64 : LibreOffice Spreadsheet Application

# yum search libreoffice-headless
# Not Found.

# Details:

# yum info libreoffice-writer.x86_64
Available Packages
Name         : libreoffice-writer
Epoch        : 1
Version      : 6.4.7.2
Release      : 5.el8
Architecture : x86_64
Size         : 3.8 M
Source       : libreoffice-6.4.7.2-5.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : LibreOffice Word Processor Application
URL          : http://www.libreoffice.org/
License      : (MPLv1.1 or LGPLv3+) and LGPLv3 and LGPLv2+ and BSD and (MPLv1.1 or GPLv2 or LGPLv2 or Netscape) and Public
             : Domain and ASL 2.0 and MPLv2.0 and CC0
Description  : The LibreOffice Word Processor application.


# yum info libreoffice-calc.x86_64
Available Packages
Name         : libreoffice-calc
Epoch        : 1
Version      : 6.4.7.2
Release      : 5.el8
Architecture : x86_64
Size         : 8.7 M
Source       : libreoffice-6.4.7.2-5.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : LibreOffice Spreadsheet Application
URL          : http://www.libreoffice.org/
License      : (MPLv1.1 or LGPLv3+) and LGPLv3 and LGPLv2+ and BSD and (MPLv1.1 or GPLv2 or LGPLv2 or Netscape) and Public
             : Domain and ASL 2.0 and MPLv2.0 and CC0
Description  : The LibreOffice Spreadsheet application.


# What other Libre Office packages are available?

# yum info libreoffice-core.x86_64
Available Packages
Name         : libreoffice-core
Epoch        : 1
Version      : 6.4.7.2
Release      : 5.el8
Architecture : x86_64
Size         : 109 M
Source       : libreoffice-6.4.7.2-5.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : Core modules for LibreOffice
URL          : http://www.libreoffice.org/
License      : (MPLv1.1 or LGPLv3+) and LGPLv3 and LGPLv2+ and BSD and (MPLv1.1 or GPLv2 or LGPLv2 or Netscape) and Public
             : Domain and ASL 2.0 and MPLv2.0 and CC0
Description  : The shared core libraries and support files for LibreOffice.

# yum info libreoffice-x11.x86_64
Available Packages
Name         : libreoffice-x11
Epoch        : 1
Version      : 6.4.7.2
Release      : 5.el8
Architecture : x86_64
Size         : 314 k
Source       : libreoffice-6.4.7.2-5.el8.src.rpm
Repository   : rhel-8-appstream-rhui-rpms
Summary      : LibreOffice generic X11 support plug-in
URL          : http://www.libreoffice.org/
License      : (MPLv1.1 or LGPLv3+) and LGPLv3 and LGPLv2+ and BSD and (MPLv1.1 or GPLv2 or LGPLv2 or Netscape) and Public
             : Domain and ASL 2.0 and MPLv2.0 and CC0
Description  : A plug-in for LibreOffice that enables generic X11 support.


# yum search libreoffice | egrep -v "langpack|help"
===================== Name & Summary Matched: libreoffice ======================
libreoffice-base.x86_64 : Database front-end for LibreOffice
libreoffice-calc.x86_64 : LibreOffice Spreadsheet Application
# libreoffice-core.x86_64 : Core modules for LibreOffice
libreoffice-data.noarch : LibreOffice data files
libreoffice-draw.x86_64 : LibreOffice Drawing Application
libreoffice-emailmerge.x86_64 : Email mail-merge component for LibreOffice
libreoffice-graphicfilter.x86_64 : LibreOffice Extra Graphic filters
libreoffice-gtk2.x86_64 : LibreOffice GTK+ 2 integration plug-in
libreoffice-gtk3.x86_64 : LibreOffice GTK+ 3 integration plug-in
libreoffice-impress.x86_64 : LibreOffice Presentation Application
libreoffice-math.x86_64 : LibreOffice Equation Editor Application
libreoffice-ogltrans.x86_64 : 3D OpenGL slide transitions for LibreOffice
libreoffice-opensymbol-fonts.noarch : LibreOffice dingbats font
libreoffice-pdfimport.x86_64 : PDF Importer for LibreOffice Draw
libreoffice-pyuno.x86_64 : Python support for LibreOffice
libreoffice-voikko.x86_64 : Finnish spellchecker and hyphenator extension for LibreOffice
libreoffice-wiki-publisher.x86_64 : Create Wiki articles on MediaWiki servers with LibreOffice
libreoffice-writer.x86_64 : LibreOffice Word Processor Application
# libreoffice-x11.x86_64 : LibreOffice generic X11 support plug-in
libreoffice-xsltfilter.x86_64 : Optional xsltfilter module for LibreOffice
libreofficekit.x86_64 : A library providing access to LibreOffice functionality
========================== Name Matched: libreoffice ===========================
libreoffice-filters.x86_64 : All import / export filters
libreoffice-gdb-debug-support.x86_64 : Additional support for debugging with gdb
libreoffice-ure.x86_64 : UNO Runtime Environment
libreoffice-ure-common.noarch : Common UNO Runtime Environment

