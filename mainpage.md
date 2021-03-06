Dummy header that will be removed by Doxygen for some reason
------------------------------------------------------------

How to use this documentation
-----------------------------

This is an API reference for programmers. Before digging into it, it is helpful
to understand the concepts of CMPI, for example by reading the introductory
chapters of the @ref ref-cmpi-standard "CMPI Standard".

The [<b>Modules</b>](modules.html) tab (at the top of this page) resembles the
heading structure of the CMPI Standard as much as possible (except for the
introductory chapters). In addition, it has modules for preprocessor symbols and
for the CMPI convenience functions (also known as CMPI macros). This tab should
be used as a general entry point, unless you know exactly what you are looking
for.

The [<b>Related Pages</b>](pages.html) tab provides automatically generated
lists, such as things added in CMPI 2.1, or things made mandatory in CMPI 2.1,
or the MB capabilities, or a list of deprecated elements.

The [<b>Data Structures</b>](annotated.html) tab provides an alphabetically
sorted list of all structures and unions of the CMPI Standard, and of their
data fields. This list does not contain any enumerations, preprocessor symbols,
or typedefs that are unrelated to structures or unions.

The [<b>Files</b>](files.html) tab lists the CMPI header files, and with each
of them, the list of data structures (structs and unions), macros (including
symbols), typedefs, and enumerations. There is also an alphabetically sorted
list of globals.

C/C++ Language Considerations and Header Files
----------------------------------------------

As stated in Subclause 4.7 of the @ref ref-cmpi-standard "CMPI Standard", CMPI
is a C Language API. The CMPI header files are usable for both C and C++. The
minimum language level that is required for CMPI is C99 (see @ref
ref-iso-iec-9899-1999 "ISO/IEC 9899:1999"). However, not all language features
of C99 are used in the CMPI header files.

The CMPI header files are:

  * `cmpift.h` - Main header file for CMPI; Defines CMPI function tables and
    object structures. MIs and MBs should include this main header file.
  * `cmpimacs.h` - Defines @ref convenience-func "CMPI convenience functions"
    that ease the use of the various function tables. MIs that intend to use the
    convenience functions need to include this header file.
  * `cmpidt.h` - Defines CMPI data types.
    MIs and MBs do not need to include this header file because it is already
    included when including the main header file `cmpift.h`.
  * `cmpios.h` - Defines OS-specific symbols for threading structures, etc.
    MIs and MBs do not need to include this header file because it is already
    included when including the main header file `cmpift.h`.
  * `cmpipl.h` - Verifies that a valid compile platform has been defined.
    MIs and MBs do not need to include this header file because it is already
    included when including the main header file `cmpift.h`.

These files are provided as a convenience only. In the case of any discrepancy
between the header files and the CMPI Standard (incorporating any subsequent
Technical Corrigenda), the CMPI Standard shall be definitive.

Some CMPI-related C preprocessor symbols can be set by users of the CMPI header
files; they are described in module @ref symbols-user
"Symbols definable by the CMPI user".

@anchor ref-cmpi-standard
CMPI 2.1.0 Standard
-------------------

  * The Open Group: Systems Management: Common Manageability Programming
    Interface (CMPI), Issue 2.1, **TBD: Release date**<br/>
    **TBD: Download link**

References
----------

  * @anchor ref-ansi-ieee-754
    ANSI/IEEE Std 754-1985: *IEEE Standard for Binary Floating-Point
    Arithmetic*, August 1985;<br/>
    http://ieeexplore.ieee.org/xpl/freeabs_all.jsp?arnumber=30711

  * @anchor ref-dmtf-dsp0004
    DMTF DSP0004: *CIM Infrastructure*, Version 2.8.0;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0004_2.8.0.pdf

  * @anchor ref-dmtf-dsp0200
    DMTF DSP0200: *CIM Operations over HTTP*, Version 1.4.0;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0200_1.4.0.pdf

  * @anchor ref-dmtf-dsp0201
    DMTF DSP0201: *Representation of CIM in XML*, Version 2.4.0;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0201_2.4.0.pdf

  * @anchor ref-dmtf-dsp0202
    DMTF DSP0202: *CIM Query Language Specification*, Version 1.0.0;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0202_1.0.0.pdf

  * @anchor ref-dmtf-dsp0212
    DMTF DSP0212: *Filter Query Language*, Version 1.0.1;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0212_1.0.1.pdf

  * @anchor ref-dmtf-dsp0223
    DMTF DSP0223: *Generic Operations*, Version 1.1.0;<br/>
    http://www.dmtf.org/standards/published_documents/DSP0223_1.1.0.pdf

  * @anchor ref-dmtf-dsp0228
    DMTF DSP0228: *Message Registry XML Schema*, Version 1.2.0;<br/>
    http://schemas.dmtf.org/wbem/messageregistry/1/dsp0228_1.2.0.xsd

  * @anchor ref-dmtf-dsp1054
    DMTF DSP1054: *Indications Profile*, Version 1.2.2;<br/>
    http://www.dmtf.org/standards/published_documents/DSP1054_1.2.2.pdf

  * @anchor ref-dmtf-dsp8016
    DMTF DSP8016: *WBEM Operations Message Registry*, Version 1.1.0;<br/>
    http://schemas.dmtf.org/wbem/messageregistry/1/dsp8016_1.1.0.xml

  * @anchor ref-ieee-1003-1
    IEEE 1003.1-2008: *Standard for Information Technology – Portable Operating
    System Interface (POSIX)*;<br/>
    http://www.opengroup.org/onlinepubs/9699919799/

  * @anchor ref-ietf-rfc-2616
    IETF RFC2616: *Hypertext Transfer Protocol – HTTP/1.1*, June 1999;<br/>
    http://tools.ietf.org/html/rfc2616

  * @anchor ref-iso-iec-646-1991
    ISO/IEC 646:1991: *Information Technology – ISO 7-bit Coded Character Set
    for Information Interchange*;<br/>
    http://www.iso.org/iso/catalogue_detail.htm?csnumber=4777

  * @anchor ref-iso-iec-9899-1999
    ISO/IEC 9899:1999: <em>(C99) Programming Languages – C</em>;<br/>
    http://www.iso.org/iso/catalogue_detail.htm?csnumber=29237
