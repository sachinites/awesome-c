# Awesome C #

A curated list of C good stuff. This list contains *only* [freedom-respecting][13]
code, and sellers who aren't evil for physical resources.

This is released under a Creative Commons-Attribution-ShareAlike license,
version 4. You can find its text in the LICENSE file.

**An important note:** This project does *not* index anything C++-related; only
pure C stuff is considered.

**Note for contributors:** If you want to make a pull request, please read
CONTRIBUTING.md first.

## Contents ##

* [AI](#ai)
* [Build Systems](#build-systems)
* [Compilers](#compilers)
* [Compression](#compression)
* [Concurrency and Parallelism](#concurrency-and-parallelism)
* [Crypto](#crypto)
* [Database](#database)
* [Debugging](#debugging)
* [Documentation Generation](#documentation-generation)
* [Editors](#editors)
* [Frameworks](#frameworks)
* [Game Programming](#game-programming)
  * [Engines](#engines)
  * [Resources](#resources)
* [Generic Programming](#generic-programming)
* [Graphics](#graphics)
* [Graphical User Interface](#graphical-user-interface)
* [Hashing](#hashing)
* [JSON](#json)
* [Learning, Reference and Tutorials](#learning-reference-and-tutorials)
  * [Reference resources online](#reference-resources-online)
  * [Beginner resources online](#beginner-resources-online)
  * [Intermediate resources online](#intermediate-resources-online)
  * [Advanced resources online](#advanced-resources-online)
  * [Online self-study courses](#online-self-study-courses)
  * [Reference books](#reference-books)
  * [Beginner books](#beginner-books)
  * [Intermediate books](#intermediate-books)
  * [Advanced books](#advanced-books)
* [Lexing and Parsing](#lexing-and-parsing)
* [Memory Management](#memory-management)
* [Multimedia](#multimedia)
* [Networking and Internet](#networking-and-internet)
  * [Web Frameworks](#web-frameworks)
* [Numerical](#numerical)
* [Profiling](#profiling)
* [Regex](#regex)
* [Serialization](#serialization)
* [Source Code Collections](#source-code-collections)
* [Standard Libraries](#standard-libraries)
* [String Manipulation](#string-manipulation)
* [Testing](#testing)
* [Text Editor Extensions](#text-editor-extensions)
  * [Emacs](#emacs)
  * [Neovim/Vim](#neovimvim)
* [Tools](#tools)
* [Utilities](#utilities)
* [Windows Environments](#windows-environments)
* [XML](#xml)

## AI ##

This includes such things as computer vision, neural nets, machine learning, and
other such things. Basically, if your university calls it AI, it lives here.

* [ccv][195] - C-based/Cached/Core Computer Vision library; modern computer
  vision. [BSD-3-Clause][6].
* [Cranium][525] - A portable, header-only ANN library in C99. [MIT][11].
* [FANN][325] - Fast Artifical Neural Network library; an implementation of
  neural networks. [GPL-2.0][8].
* [Genann][412] - A simple ANN in C89, without additional dependencies. [Zlib][49].
* [libdeep][477] - A deep learning library. [BSD-3-Clause][6].

## Build Systems ##

These are tools to automate the building and testing of projects in C.

* [Autoconf][305] - An extensible package of M4 macros that produce shell
  scripts to automatically configure software source code packages. Part of the
  Autotools. [GPL-3.0+][41].
* [Automake][306] - A tool for automatically generating ``Makefile.in`` files
  compliant with the GNU Coding Standards. Requires the use of Autoconf. Part of
  the Autotools. [GPL-3.0+][41].
* [GNU Make][324] - A tool which controls the generation of executables and other
  non-source files of a program. [GPL-3.0+][41].
* [Libtool][172] - A generic library support script. Part of the
  Autotools. [GPL-3.0+][41].
* [Meson][368] - An extremely fast, user-friendly build system. Based on Ninja. [Apache-2.0][32].
* [Premake][435] - A command-line utility which reads a scripted definition of a
  software project and uses it to generate project files for Visual Studio and
  GNU Make. Other targets are also being worked on. [BSD-3-Clause][6].
* [tup][326] - A very fast, file-based, cross-platform build
  system. [GPL-2.0][8].
* [zproject][420] - A project generator and build system support.
  [MPL-2.0][227].

## Compilers ##

This section also includes compiler-related and compilation-related tooling.

* [ccache][466] - A compiler cache designed to speed up recompilation. [GPL-3.0+][41].
* [Clang][38] - A compiler for LLVM. Supports C11. [NCSA][39].
* [distcc][452] - A program to allow builds to be distributed among several
  machines. [GPL-2.0+][8].
* [GCC][40] - Provides a C compiler as part of its compiler set. Supports
  C11. [GPL-3.0+][41].
* [PCC][74] - A venerable compiler. Supports C99. [Various licenses][75], all free.

## Compression ##

* [blosc][445] - An extremely fast, multi-threaded, meta-compressor
  library. Various licenses, all free.
* [clzip][432] - C version of the high-quality data compressor [Lzip][433] (LZMA
  implementation). [GPL-2.0+][8].
* [CRoaring][481] - C implementation of [Roaring bitmaps][482]. [Apache-2.0][32].
* [DENSITY][506] - A super-fast compression library. [BSD-3-Clause][6].
* [heatshrink][514] - A data compression/decompression library for embedded and
  real-time systems. [ISC][61].
* [huffandpuff][214] - A minimal Huffman encoder and decoder. Public domain.
* [libbzip2][427] - A patent-free, high-quality data compression
  library. [BSD-4-Clause][310].
* [lz4][508] - Library for an extremely fast compression algorithm.
  [BSD-2-Clause][24].
* [lzo][338] - A very fast data compression library. [GPL-2.0+][8].
* [shoco][363] - A compressor for small text strings. [MIT][11].
* [SIMDComp][519] - A simple library for compressing lists of integers using
  binary packing. Makes use of SIMD instructions on x86. [BSD-3-Clause][6].
* [smaz][364] - An efficient string compression library. [BSD-3-Clause][6].
* [squash][393] - A compression abstraction library, complete with some
  utilities. [MIT][11].
* [TurboPFor][471] - Fastest integer compression. [GPL-2.0+][8].
* [TurboRLE][484] - Most efficient run-length encoding. [GPL-2.0+][8].
* [zip][520] - A really really small zip archive processing library.
  [Unlicense][521].
* [Zlib][230] - A massively-spiffy yet delicately-unobtrusive compression
  library. [BSD-3-Clause][6].
* [Zstandard][510] - A fast, lossless compression algorithm, targeting real-time
  compression scenarios at zlib-level or better compression ratios.
  [BSD-3-Clause][6].

## Concurrency and Parallelism ##

* [cchan][243] - A small library for channel constructs for inter-thread
  communication. Public domain.
* [cf4ocl][311] - The C Framework for OpenCL; a cross-platform object-oriented
  framework for developing and benchmarking [OpenCL][312] projects. 
  [LGPL-3.0][5].
* [checkedthreads][465] - No race condition goes unnoticed! A simple library for
  parallelism, with built-in checking for race conditions. [BSD-2-Clause][24].
* [ck][242] - Concurrency primitives, safe memory reclamation mechanisms and
  non-blocking data structures. [BSD-2-Clause][24].
* [libconcurrent][390] - Concurrent programming library, using coroutines, for
  C11. [BSD-3-Clause][6].
* [libdill][442] - A library which makes structured concurrent programming
  easy. [MIT][11].
* [libhl][478] - A library implementing a thread-safe API to manage a range of data
  structures. Also provides some supporting functions and structures for
  concurrent and lockfree programming. [LGPL-3.0][5].
* [liburcu][474] - A data synchronization library, which scales linearly with the
  number of cores. [LGPL-2.1+][15].
* [mill][352] - Go-style concurrency. [MIT][11].
* [OpenMP][37] - A set of pragmas designed to allow for easy parallelization of
  code. Standard (licensing not applicable).
* [OpenMPI][284] - A message passing interface implementation. [BSD-3-Clause][6].
* [pal][459] - An optimized library for maths, parallel processing and data
  movement. [Apache-2.0][32].
* [PETSc][282] - A suite of data structures and routines for scalable parallel
  solution of scientific applications modelled by partial differential
  equations. [BSD-2-Clause][24].
* [pth][180] - A portable implementation for non-preemptive priority-based
  scheduling for multiple threads of execution. [GPL-3.0+][41].
* [pthreads][146] - The POSIX thread library. Standard (no license applicable).
* [TinyCThread][115] - A portable, small implementation of the C11 threads
  API. [Zlib][49].

## Crypto ##

This is mostly library implementations of well-known cryptographic algorithms or
protocols.

* [GNU SASL][160] - An implementation of the Simple Authentication and Security
  Layer and a few common SASL mechanism. [GPL-3.0+][41].
* [GnuTLS][112] - A secure communication library, implementing SSL, TLS and
  DTLS. [LGPL-2.1+][15].
* [libgcrypt][142] - A general-purpose cryptography library, with a range of
  available ciphers. [LGPL-2.1+][15].
* [OpenSSL][110] - Implementation of the SSL and TLS protocols. Also includes a
  cryptography
  library. [Dual Licensed under the OpenSSL License and the SSLeay License][111].
* [liboqs][493] - A library for quantum-resistant cryptographicl algorithms.
  [MIT][11].
* [libsodium][198] - A modern and easy-to-use crypto library. [MIT][11].
* [libtomcrypt][299] - A fairly comprehensive, modular and portable
  cryptographic toolkit. Public domain.
* [mbed TLS][291] - Another crypto implementation. [Apache-2.0][32].
* [MIRACL][480] - Multiprecision Integer and Rational Arithmetic Cryptographic
  Library; an SDK for elliptic curve cryptography. [AGPL-1.0+][381].
* [retter][507] - A collection of hash functions, ciphers, tools, libraries and
  materials related to cryptography and security. Public domain.
* [s2n][359] - A C99 implementation of the TLS/SSL protocols, designed to be
  simple, fast and with security as a priority. [Apache-2.0][32].
* [sphlib][526] - A set of implementations of various hash functions, including
  several cryptographic ones. [MIT][11].

## Database ##

This lists databases and data stores with C APIs.

* [BerkeleyDB][380] - A library for a high-performance embedded database for
  key-value data. [AGPL-1.0][381].
* [Groonga][524] - Columnar store with full-text search. [LGPL-2.1][15].
* [Hiredis][201] - A minimalistic client library for Redis. [BSD-3-Clause][6].
* [libmongoc][233] - A high-performance client library for [MongoDB][234]. [Apache-2.0][32].
* [LMDB][105] - An ultra-fast, ultra-compact key-value embedded data store. [OLDAP-2.8][106].
* [MariaDB][25] - A robust, scalable and reliable SQL server, designed to be a
  drop-in replacement for MySQL. [BSD-3-Clause][6].
* [PostgreSQL][121] - A powerful object-relational database system. [PostgreSQL][122].
* [recutils][360] - A set of tools and a library for accessing human-editable,
  plaintext database files called recfiles. [GPL-3.0+][41].
* [Redis][51] - An advanced key-value store. [BSD-3-Clause][6].
* [sophia][244] - A modern, embeddable key-value database. [BSD-2-Clause][24].
* [sparkey][509] - A simple constant key/value storage library. Designed for
  read-heavy loads with infrequent, large bulk inserts. [Apache-2.0][32].
* [SQLite][22] - A self-contained, serverless, zero-configuration, transactional
  SQL database engine. Public domain.
* [UnQLite][23] - A self-contained, serverless, zero-configuration,
  transactional NoSQL engine. [BSD-2-Clause][24].
* [WhiteDB][512] - A lightweight database library, operating entirely in main
  memory. [GPL-3.0+][41].

## Debugging ##

Because we all have to do it sometimes. This includes various tools for making
debugging easier or better, as well as libraries or code that allows better
debugging work.

* [C-Reduce][403] - A tool that takes a large C file with a property of interest
  and automatically produces a much smaller C file that has the same
  property. Intended to help create minimal bug-demonstrating cases in complex
  code. [BSD-3-Clause][6].
* [CBMC][309] - C Bounded Model Checker; a tool for verification of array
  bounds, pointer safety and user-specified assertions. [BSD-4-Clause][310].
* [cflow][404] - Analyzes a collection of source files and prints a graph
  charting control flow in the program. [GPL-3.0+][41].
* [Complexity][307] - A tool for measuring the complexity of source
  code. [GPL-3.0+][41].
* [CScout][410] - A source code analyzer and refactoring browser for C
  programs. [GPL-3.0][41].
* [DDD][320] - A graphical front-end for a range of command-line
  debuggers. [GPL-3.0+][41].
* [debug][467] - A one-header library for easier 'printf debugging'.
  [MIT][11].
* [GDB][87] - The GNU Project debugger. [GPL-3.0+][41].
* [lldb][468] - The LLVM debugger. [NCSA][39].
* [rr][95] - A debugger that records non-deterministic executions to allow for
  deterministic debugging. [BSD-2-Clause][24].
* [Valgrind][85] - A range of dynamic analysis tools, including a leak
  checker. [GPL-2.0][8].

## Documentation Generation ##

* [Cxref][317] - Generates documentation in either LaTeX, HTML, RTF or
  SGML. [GPL-2.0][8].
* [DocOnce][322] - A modestly-tagged markup language that can be used to
  generate a range of formats. [BSD-3-Clause][6].
* [Doxygen][318] - The de-facto standard tool for generating documentation from
  annotated sources. Can generate a large range of formats. [GPL-2.0][8].
* [GTK-Doc][319] - A tool for generating documentation from annotated
  sources. Has support for the Autotools. [GPL-2.0][15].

## Editors ##

These are specifically fancier, IDE-type editors. If you want a programmer's
text editor, look elsewhere. Besides, whatever choice you make most likely
supports C anyway.

* [Anjuta DevStudio][42] - The GNOME IDE. [GPL-2.0][15].
* [Code::Blocks][249] - An extensible, configurable IDE supporting
  C. [GPL-3.0][41].
* [CodeLite][45] - A cross-platform IDE. [GPL-2.0][8].
* [Eclipse][258] - An IDE written in Java. [EPL][259].
* [Geany][43] - A very small and fast IDE. [GPL-2.0+][8].
* [KDevelop][44] - The KDE IDE. [GPL-2.0][8].

## Frameworks ##

This section has big libraries that provide data structures and other stuff you
expect of a 'modern' standard library.

* [APR][78] - Apache Portable Runtime; another library of cross-platform utility
  functions. [Apache-2.0][32].
* [C Algorithms][88] - A collection of common algorithms and data structures. [ISC][61].
* [Collections-C][406] - A library of generic data structures. [LGPL-3.0+][5].
* [CPL][308] - The Common Pipeline Library; a set of libraries designed to be a
  comprehensive, efficient and robust software toolkit. [GPL-2.0][8].
* [EFL][119] - A large collection of useful data structures and
  functions. Various licenses, all free.
* [GLib][1] - A library of utility functions and structures, designed to be
  portable, efficient and powerful. [LGPL-2.1][15].
* [GIO][2] - A modern and easy-to-use VFS API. [LGPL-2.1][15].
* [GObject][3] - An object-oriented system and object model. [LGPL-2.1][15].
* [libcork][476] - Utility functions and structures, designed for
  resource-constrained systems. Can be embedded. [BSD-3-Clause][6].
* [libnih][93] - A lightweight library of functions and
  structures. [GPL-2.0][8].
* [libU][28] - A small library of basic utilities, including memory allocation,
  string manipulation and logging. [BSD-3-Clause][6].
* [offbrand][498] - A collection of generic, reference-counted data structures.
  [MIT][11].
* [PBL][346] - A large library of utilities, featuring data structures, among
  other things. [LGPL-2.1+][15]. 
* [qlibc][277] - A simple and powerful library, designed as a replacement for
  GLib while focusing on being small and light. [BSD-2-Clause][24].
* [stb][114] - A range of single-file libraries. Public domain.
* [TBOX][398] - A multi-platform library with a large number of
  capabilities. [LGPL-2.1+][15].

## Game Programming ##

### Engines ###

These are provided as examples of C game programming code.

* [Corange][101] - A game engine in pure C. [BSD-2-Clause][24].
* [Darkplaces][369] - A modified version of the Quake2 engine. [GPL-2.0][8].
* [ioquake3][107] - The Quake3 engine, freed at last. [GPL-2.0][8].
* [Orx][370] - A portable, lightweight, plugin-based, data-driven, 2D-oriented
  game engine. [Zlib][49].
* [Quake][225] - The Quake engine. [GPL-2.0][8].
* [Quake2][221] - The Quake2 engine. [GPL-2.0][8].
* [Spearmint][371] - An engine designed for FPS games. [GPL-3.0+][41].

### Resources ###

These are libraries of all sorts that are useful for game programming.

* [Allegro][48] - A cross-platform, video game development and multimedia
  library. [Zlib][49].
* [Chipmunk2D][303] - A fast and lightweight 2D game physics library. [MIT][11].
* [CSFML][90] - A binding for [SFML][91]. [Zlib][49].
* [Epoxy][414] - A library for handling OpenGL function pointer management. [MIT][11].
* [FreeGLUT][99] - An alternative to the OpenGL Utility Toolkit. Allows the
  creation and management of windows with OpenGL contexts. [X11][100].
* [GLFW][98] - A multi-platform library for creating windows with OpenGL
  contexts. [Zlib][49].
* [kazmath][446] - A maths library for games. [BSD-2-Clause][24].
* [libao][376] - A cross-platform audio library with a wide variety of
  outputs. [GPL-2.0+][8].
* [raylib][516] - A simple and easy-to-use library to learn video game
  programming. [Zlib][49].
* [RetroArch][231] - The reference frontend for [libretro][232]. [GPL-3.0][41].
* [SDL2][50] - A cross-platform library designed to provide low-level access to
  audio, keyboard, mouse, joystick and graphics hardware via OpenGL. [Zlib][49].
* [sdl-gpu][457] - A library for high-performance, modern 2D graphics. Based on
  SDL. [MIT][11].
* [SIGIL][429] - Sound, Input and Graphics Integration Library; a simple
  alternative to other libraries for doing all those things. Various licenses,
  all free.

## Generic Programming ##

* [klib][76] - Small and lightweight implementations of common algorithms and
  data structures. [MIT][11].
* [SGLIB][30] - A simple generic library. Any OSI-approved license.

## Graphics ##

* [Cairo][384] - A 2D graphics library. [LGPL-2.1][15] or [MPL-1.1][385].
* [Cogl][127] - A GPU graphics and utilities API. [MIT][11]. 
* [Clutter][126] - A UI library based on OpenGL. [LGPL-2.1][15].
* [giflib][401] - A library for reading and writing gif images. [MIT][11].
* [graphene][515] - A thin layer of graphical data types. [MIT][11].
* [heman][365] - A tiny library of image utilities dealing with height maps,
  normal maps, distance fields and the like. [MIT][11].
* [libcaca][366] - An ASCII renderer for terminal-based interfaces. [WTFPL][367].
* [libgd][402] - A library for the dynamic creation of images by programmers. [MIT][11].
* [libimagequant][300] - Small, portable library for high-quality conversion of
  RGBA images to 8-bit indexed colour images. [GPL-3.0+][41].
* [libjpeg-turbo][193] - A faster library for reading and writing JPEG
  files. [Various licences][194].
* [libpng][382] - The official PNG reference library. [Libpng][383].
* [libRSVG][417] - A library to render SVG files using Cairo. [LGPL-2.1+][15].
* [libsixel][17] - A library implementing the SIXEL protocol, allowing beautiful
  graphics in your terminal. [MIT][11].
* [libvips][511] - An image processing library. [LGPL-2.1+][15].
* [libxmi][174] - A function library for rasterizing 2D vector
  graphics. [GPL-3.0+][41].
* [lightmapper][444] - A single-file library for lightmap baking, using an
  existing OpenGL renderer. Public domain.
* [mozjpeg][200] - An improved JPEG encoder. [BSD-3-Clause][6].
* [nanovg][505] - Anti-aliased 2D vector drawing library on top of OpenGL, for
  UI and visualizations. [Zlib][49].
* [OpenGL][147] - The industry standard for high-performance graphics, with a
  native C binding. [Various licenses][148].

## Graphical User Interface ##

These are specifically [widget toolkits][12], or things meant to be used in a
similar way to them.

* [GTK+][14] - A cross-platform widget toolkit. [LGPL-2.1][15].
* [IUP][16] - Another cross-platform widget toolkit. [MIT][11].
* [nuklear][408] - A small, C89, single-header widget toolkit. Public domain.
* [tinyfiledialogs][426] - A single-file library for simple dialogs. Compatible
  with many other toolkits and OSes. [Zlib][49].
* [Tk][19] - A basic widget toolkit. Part of Tcl/Tk. [TCL][20].
* [XForms Toolkit][21] - A widget toolkit designed for the XWindow
  system. [LGPL-2.1][15].

## Hashing ##

These are hash function implementations for *non*-crypto purposes.
Cryptographic hashes can be found in the Crypto section.

* [CLHash][495] - A library implementing the ridiculously fast CLHash hashing
  function. Only works on Intel Haswell or newer. [Apache-2.0][32].
* [HighwayHash][527] - A fast, strong, SIMD-using hash function. Also contains
  an implementation of SipHash (although this is slower). [Apache-2.0][32].
* [xxHash][522] - An extremely fast hashing algorithm. Comes in 32 and 64-bit
  varieties. [BSD-2-Clause][24].

## JSON ##

* [cJSON][443] - Ultra-lightweight JSON parser. [MIT][11].
* [Jansson][53] - A library for encoding, decoding and manipulating JSON. [MIT][11].
* [jsmn][120] - A minimalistic JSON parser. [MIT][11].
* [jfes][488] - A simple JSON engine without any dependencies. [MIT][11].
* [json-c][220] - A library for working with JSON. [MIT][11].
* [WJElement][77] - Advanced JSON manipulation library, with support for JSON
  Schema. [LGPL-2.0+][334] or [LGPL-2.1+][15] or [LGPL-3.0+][5]. 
* [YAJL][60] - A fast streaming JSON parser library. [ISC][61]

## Learning, Reference and Tutorials ##

This is a list of resources for learning C programming in general, or something
useful relating to C programming.

### Reference resources online ###

* [Benchmarks of the Lockless Memory Allocator][450] (compares to other
  implementations)
* [C FAQ - comp.lang.c Frequently Asked Questions][262]
* [Comparison of C/POSIX standard library implementations for GNU/Linux][362]
* [Draft C11 standard][247]
* [Finding the best 64-bit simulation PRNG][529]
* [GNU C Reference Manual][329]
* [Robert Pike's notes on programming in C][273]
* [SEI CERT C Coding Standard][266]

### Beginner resources online ###

* [A tutorial on pointers][213]
* [A tutorial on portable Makefiles][528]
* [Building C Projects][208]
* [C Programming Wikibook][248]
* [Introduction to \`fun' C][279]
* [Learning C with GDB][349]
* [POSIX Threads Programming tutorial][263] (a little dated, but most of it is
  still valid and useful)
* [The GNU C Programming Tutorial][212] (online PDF)
* [Templating in C][267]

### Intermediate resources online ###

* [8 gdb tricks you should know][206]
* [10 C99 tricks][257]
* [A comprehensive MPI tutorial resource][454]
* [Bit Twiddling Hacks][530]
* [Diving into concurrency: trying out mutexes and atomics][202]
* [Introduction to OpenMP][207] (video)
* [OpenMP tutorial][264] (for the OpenMP3 standard)
* [memcpy vs memmove][205]
* [MPI tutorial][265]
* [Scalable C - Writing Large-Scale Distributed C][391]
* [Some unknown features or tricks in C language][374]
* [What a C programmer should know about memory][271]
* [What every C programmer should know about undefined behaviour][275]

### Advanced resources online ###

* [Advanced metaprogramming in C][357]
* [A quick tutorial on implementing and debugging malloc, free, calloc, and realloc][204]
* [Bit twiddling hacks][73]
* [I do not know C][272]
* [Implementing smart pointers for the C programming language][240]
* [Inline functions in C][245]
* [Metaprogramming custom control structures in C][343]
* [Solving the temporary storage problem of C macros][358]
* [Some dark corners of C][210]
* [Writing efficient C and C code optimization][33]

### Online self-study courses ###

* [C Programming Language Certified Associate preparation course][211]

### Reference books ###

* [C: A Reference Manual 5E][181] - A full reference book for C99.
* [C in a Nushell 2E][418] - A concise reference book for C11.
* [C Pocket Reference][182] - A concise reference book for C99.
* [The C Programming Language 2E][7] - The original book on C, by its creators.

### Beginner books ###

* [C Primer Plus 6E][184] - A complete tutorial on programming in C11.
* [C Programming: A Modern Approach][64] - An excellent book to learn the basics
  from C from.
* [Head First C][102] - A 'head-first' style book for learning C.

### Intermediate books ###

* [21st Century C][35] - A very good *second* programming book on C.
* [Understanding and Using C Pointers][36] - An in-depth resource on pointers in
  C.
* [ZeroMQ][183] - A book for using ZeroMQ with C.

### Advanced books ###

* [Expert C Programming: Deep C Secrets][55] - An interesting, in-depth and
  *entertaining* look at the innards of C.

## Lexing and Parsing ##

This details libraries specifically for [lexical analysis][489] (or lexing) and
[syntactic analysis][490] (or parsing).

* [flex][491] - The fast lexical analyzer generator. [BSD-2-Clause][24].
* [GNU Bison][492] - A general-purpose parser generator that converts an
  annotated context-free grammar into a range of parsers. [GPL-3.0+][41].
* [hammer][356] - Parser combinators for binary formats. [GPL-2.0][8].
* [mpc][238] - A parser combinator library. [BSD-2-Clause][24].
* [re2c][34] - A lexer generator, producing very fast lexers, with access to its
  internals. Public domain.

## Memory Management ##

Whether a different, faster ``malloc`` or outright garbage collection, anything
to do with managing C memory lives here.

* [Boehm GC][125] - Garbage collection for C? Don't mind if I do! Various
  licenses, all free.
* [jemalloc][293] - A malloc implementation that emphasizes avoidance of
  fragmentation and scalable concurrency support. [BSD-2-Clause][24].
* [Lockless Memory Allocator][451] - An efficient memory allocator. [GPL-3.0+][41].
* [talloc][353] - A hierarchical, reference-counted memory pool system with
  destructors. [LGPL-3.0+][5].

## Multimedia ##

* [aubio][523] - A library for audio and music analysis. [GPL-3.0+][41].
* [FFMPEG][63] - A complete, cross-platform solution to record, convert and
  stream audio and video. [LGPL-2.1+][15]
* [GStreamer][123] - A framework for audio and visual media. [LGPL-2.1+][15].
* [libmpv][348] - A music-playing library. Compile with ``./waf configure
  --disable-cplayer --enable-libmpv-shared`` to not have the music
  player. [GPL-2.0+][8].
* [libsndfile][458] - A library for reading and writing sound files. Supports
  many formats. [LGPL-2.1][15] or [LGPL-3.0][5].
* [libsoundio][372] - A library for cross-platform, real-time audio input and
  output. Has a range of back-ends. [MIT][11].
* [lodepng][69] - A simple PNG image decoder and encoder, requiring no other
  dependencies. [BSD-3-Clause][6].
* [Soundpipe][513] - A lightweight music DSP library. [MIT][11].

## Networking and Internet ##

* [asnlc][138] - A compiler of ASN.1 specifications into C source code. [BSD-2-Clause][24].
* [CHL][422] - C Hypertext Library - A library for writing web applications in
  C. [GPL-3.0][41].
* [czmq][226] - A high-level binding for ZeroMQ. [MPL-2.0][227]
* [GNU adns][155] - An advanced, easy-to-use, asynch-capable DNS client library
  and utilities. [GPL-3.0+][41].
* [gumbo-parser][196] - An HTML5 parsing library in C99. [Apache-2.0][32].
* [http-parser][197] - An HTTP request/response parser. [MIT][11].
* [ldns][339] - A library to simplify DNS programming. [BSD-3-Clause][6].
* [libcurl][65] - A client-side URL transfer library, supporting a wide range of
  formats. [curl][66].
* [LibEtPan][222] - A mail library providing an efficient network for IMAP,
  SMTP, POP and NNTP. [BSD-3-Clause][6].
* [libev][144] - Yet another event loop. [BSD-2-Clause][24].
* [libevent][124] - An event loop replacement for network servers. [BSD-3-Clause][6].
* [libhttpd][166] - A library to add basic web server capabilities to an
  application or embedded device. [GPL-2.0][41].
* [libidn][164] - An implementation of the Stringprep, Punycode and IDNA
  specifications. [GPL-3.0+][41].
* [libmicrohttpd][165] - A small library that makes it easy to run an HTTP
  server as part of another application. [LGPL-2.1+][15].
* [libonion][170] - HTTP server library, designed to be easy to
  use. [Apache-2.0][32].
* [libquickmail][399] - A library intended to give developers a way to send
  email from their applications. Supports multiple To/Cc/Bcc recipients and
  attachments without size limits. [GPL-3.0+][41].
* [libsoup][167] - A GNOME HTTP client/server library. Uses
  GObject. [LGPL-2.1][15].
* [LibVNCServer][464] - Cross-platform libraries to implement VNC server and/or
  client functionality. [GPL-2.0+][8].
* [libwebsock][261] - An easy-to-use and powerful web socket library.
  [LGPL-3.0][5].
* [lwan][199] - An experimental, scalable, high-performance HTTP
  server. [GPL-2.0][8].
* [mongoose][171] - Embedded web server. [GPL-2.0][8].
* [nanomsg][139] - A C-based implementation of ZeroMQ. [MIT][11].
* [oSip][179] - A SIP implementation without additional
  dependencies. [LGPL-2.1+][15].
* [socket99][203] - A C99 wrapper for the BSD sockets API. [ISC][61].
* [twitc][237] - A mini library for interacting with the Twitter OAuth API. [MIT][11].
* [trezor-crypto][485] - Heavily-optimized crypto algorithms for embedded
  devices. [MIT][11].
* [Wslay][460] - A WebSocket library. Implements version 13 of the WebSocket
  protocol, as described in RFC 6455. [MIT][11].
* [zyre][419] - A framework for proximity-based peer-to-peer applications. [MPL-2.0][227].

### Web Frameworks ###

* [balde][386] - A microframework based on GLib. [LGPL-2.1][15].
* [facil.io][118] - A mini-framework for web applications. Includes a fast HTTP and
  Websocket server, and also supports custom protocols. [MIT][11].
* [KLone][423] - A fully-featured, multi-platform, web application development
  framework, targeted especially at embedded systems and
  appliances. [BSD-3-Clause][6].
* [Kore][415] - An easy-to-use web application framework for writing scalable
  web APIs in C. [ISC][61].

## Numerical ##

* [apophenia][188] - A library for statistical and scientific
  computing. [GPL-2.0][8].
* [Arb][497] - Library for arbitrary-precision interval arithmetic.
  [LGPL-2.1+][15].
* [ATLAS][137] - Automatically Tuned Linear Algebra Software. [BSD-3-Clause][6].
* [clBLAS][439] - BLAS functions written in OpenCL. [Apache-2.0][32].
* [Cuba][316] - A library for multidimensional numerical
  integration. [LGPL-3.0][5].
* [FFTW][70] - The Fastest Fourier Transform in the West; a highly-optimized
  fast Fourier transform routine. [GPL-2.0+][8].
* [FLINT][255] - Fast Library for Number Theory; a library supporting arithmetic
  with numbers, polynomials, power series and matrices, among
  others. [GPL-2.0+][8].
* [GLPK][159] - GNU Linear Programming Kit; a package designed for solving
  large-scale linear programming, mixed integer programming and other related
  problems. [GPL-3.0+][41].
* [GMP][79] - GNU Multple Precision Arithmetic Library; a library for
  arbitrary-precision arithmetic. [GPL-2.0][8] or [LGPL-3.0][5].
* [GNU MPC][175] - A library for complex number arithmetic. [LGPL-3.0+][5].
* [GNU MPFR][176] - A library for arbitrary-precision floating-point
  arithmetic. [LGPL-3.0+][5].
* [GNU MPRIA][177] - A portable mathematics library for multi-precision rational
  interval arithmetic. [GPL-3.0+][41].
* [GSL][47] - The GNU Scientific Library; a sophisticated numerical
  library. [GPL-3.0][41].
* [KISS FFT][71] - A very simple fast Fourier transform library. [BSD-3-Clause][6].
* [LAPACKE][133] - An interface to [LAPACK][134]. [BSD-3-Clause][6].
* [LibTomMath][461] - A portable, number-theoretic, multiple-precision integer
  library. Supports algebra, digit manipulation, modular reductions, and various
  number-theoretic routines. Public domain.
* [LibTomPoly][463] - A polynomial-related maths library. Public domain.
* [PARI/GP][256] - A computer algebra system for number theory; includes a
  compiler to C. [GPL-2.0+][8].
* [PETSc][282] - A suite of data structures and routines for scalable parallel
  solution of scientific applications modelled by partial differential
  equations. [BSD-2-Clause][24].
* [SCS][483] - Splitting Conic Solver; a numerical optimization package for
  solving large-scale convex cone problems. [MIT][11].
* [SLEPc][283] - A software library for the solution of large, sparse eigenvalue
  problems on parallel computers. [LGPL-3.0][5].
* [TomsFastMath][462] - A set of assembly-level-optimized maths operations,
  suitable for cryptographic use. Public domain.
* [Yeppp!][72] - Very fast, SIMD-optimized mathematical library. [BSD-3-Clause][6].

## Profiling ##

* [gperftools][295] - A collection of utilities for measuring and improving
  performance. [BSD-3-Clause][6].
* [gprof][86] - A performance analysis tool. Part of GNU binutils. 
  [GPL-3.0+][41].
* [OProfile][475] - A statistical profiler for GNU/Linux. Can profile any code
  (including the kernel!) with low overhead and without recompilation. [GPL-2.0][8].
* [perf][375] - A Linux kernel-based profiler with a lot of functionality.
  [GPL-2.0][8].

## Regex ##

> "Some people, when confronted with a problem, think 'I know, I'll use regular
> expressions'. Now they have two problems." - Jamie Zawinski.

* [Onigmo][518] - A fork of Oniguruma, supporting more advanced regexps.
  [BSD-2-Clause][24].
* [Oniguruma][517] - A regex library supporting a wide range of encodings, and
  incorporating many security-oriented fixes. [BSD-2-Clause][24].
* [PCRE][83] - An implementation of regexes identical to that of
  Perl 5. [BSD-3-Clause][6].
* [SLRE][80] - Super Light Regular Expression library; a very small
  implementation of a subset of Perl regex syntax. [GPL-2.0][8].
* [TRE][82] - A POSIX-compliant, feature-full regex library. [BSD-2-Clause][24].

## Serialization ##

* [binn][400] - A binary serialization format, meant to be compact, fast and
  easy-to-use. [Apache-2.0][32].
* [c-capnproto][130] - An implementation of the Cap'n Proto serialization
  protocol. [MIT][11].
* [cmp][377] - An implementation of the [MessagePack][379] serialization
  protocol. [MIT][11].
* [flatcc][187] - [FlatBuffers][145] compiler and library. [Apache-2.0][32].
* [libavro][140] - An implementation of the Avro data serialization system. [Apache-2.0][32].
* [mpack][378] - Another implementation of the [MessagePack][379] serialization
  protocol. [MIT][11].
* [OPIC][397] - Object Persistence in C; a revolutionary serialization framework,
  with matching on-disk and in-memory representations. [GPL-3.0+][41].
* [protobuf-c][129] - An implementation of Google Protocol Buffer. [BSD-2-Clause][24].
* [tpl][473] - A small binary serialization library. [MIT][11].
* [xdr][131] - External Data Representation; a standard for data
  serialization. Standard (no license applicable).

## Source Code Collections ##

This contains collections of small source code. If you want something big and
integrated, check the Frameworks section.

* [CCAN][103] - Modelled after Perl's CPAN, this is a big collection of code
  that does stuff. The full list is [here][104]. Various licenses, all free.
* [clib][26] - Something of a package manager. Comes with
  a [bunch of libraries of its own][27]. [MIT][11].
* [gnulib][46] - A collection of common GNU code. Various licenses, all free.
* [libdjb][292] - A collection of libraries doing various things. (Apparently)
  public domain.
* [par][456] - A bunch of single-file libraries. [MIT][11].

## Standard Libraries ##

This contains standard C libraries.

* [Bionic][4] - Google's standard library, developed for Android. [BSD-3-Clause][6].
* [cloudlibc][486] - A standard library based on the concept of
  [capability-based security][487]. [BSD-2-Clause][24].
* [dietlibc][9] - A standard library designed for the smallest possible
  binaries. [GPL-2.0][8].
* [glibc][57] - The GNU C Library; an implementation of the standard
  library. [LGPL-2.1][15].
* [PDCLib][447] - The Public Domain C Library. Implements most of C99 and some of
  C11. [CC0][448].
* [musl][10] - A standard library, compatible with POSIX 2008 and C11. Designed
  for static linking. [MIT][11].

## String Manipulation ##

* [bstrlib][116] - The Better String Library. [BSD-3-Clause][6] or [GPL-2.0][8].
* [ICU][67] - International Components for Unicode; a library for Unicode
  support. [ICU][68].
* [libunistring][173] - A library for manipulating Unicode
  strings. [LGPL-3.0][5].
* [libgiconv][163] - A text conversion library. [LGPL-2.1][15]. 
* [librope][479] - A UTF-8 rope ('heavy' string) library. [MIT][11].
* [SDS][29] - Simple Dynamic Strings; a library for handling strings in a
  simpler way, but one that is compatible with normal C string
  functions. Available via [clib][26]. [BSD-2-Clause][24].
* [utf8.h][472] - Single-header UTF-8 library, designed to mimic C-style string
  functions. Public domain.
* [utf8proc][469] - A library for processing UTF-8 data. [MIT][11].

## Testing ##

* [CHEAT][84] - A very simple unit testing framework. [BSD-2-Clause][24].
* [Check][59] - A unit testing framework. [LGPL-2.1][15].
* [clar][470] - A clear and simple unit testing framework. [MIT][11].
* [CMock][297] - A mock/stub generator. [MIT][11].
* [cmocka][141] - A unit testing framework with support for mock objects. [Apache-2.0][32].
* [Criterion][246] - A KISS, non-intrusive test framework. [MIT][11].
* [ctest][503] - Yet another unit testing framework. [Apache-2.0][32].
* [CUnit][94] - Another unit testing framework. [LGPL-2.1+][15].
* [greatest][58] - A unit testing library in one file, with no memory
  allocation. [MIT][11].
* [minctest][394] - A unit testing microlibrary. [BSD-3-Clause][6].
* [minunit][92] - Minimal unit testing framework. [MIT][11].
* [munit][392] - A small unit testing framework. [MIT][11].
* [theft][302] - Property-based testing (similar to [Quickcheck][301]). [MIT][11].
* [Unity][296] - A simple unit testing framework. [MIT][11].

## Text Editor Extensions ##

While practically any decent programmer's text editor supports C, there are some
extensions that make it more pleasant. This is categorized by editor.

### Emacs ###

* [CEDET][250] - Collection of Emacs Development Environment Tools; designed to
  provide IDE-like features to Emacs. Built-in. [GPL-3.0+][41].
* [Flycheck][149] - Modern syntax checking. For C, it can use either GCC or
  Clang as a back-end. [GPL-3.0+][41].
* [YASnippet][150] - A template system, with C templates for common code
  snippets. [GPL-3.0+][41].

### Neovim/Vim ###

* [Neomake][441] - Async :make and linting framework for Neovim/Vim. [MIT][11].
* [Syntastic][186] - Syntax checking and linting. [WTFPL][367].
* [YouCompleteMe][151] - A code completion engine for Vim. [GPL-3.0][41].

## Tools ##

This is a list of useful programs to help you write and debug C code which are
*not* editors, libraries or compilers.

* [Artistic Style][314] - A fast and small automatic source code formatter that
  supports C. [LGPL-3.0][5].
* [address-sanitizer][288] - A fast memory error detector. [Apache-2.0][32].
* [biicode][304] - A modern dependency manager. [MIT][11].
* [c][276] - Compile and execute C "scripts" in one go on the command line. Also
  has shebang support. [MIT][11].
* [c99sh][113] - Run C files using hash-bang. [BSD-2-Clause][24].
* [cdecl][347] - An online service to translate C declarations into English and
  vice versa. Public domain.
* [cinclude2dot][280] - Graphs include dependencies in a project using
  Graphviz. [GPL-1.0+][335] or [GPL-2.0+][8] or [GPL-3.0+][41].
* [ClangCheck][502] - A static analysis tool, designed to work with Clang.
  [NCSA][39].
* [Cppcheck][501] - A static analysis tool. Despite the name, works well with C.
  [GPL-3.0+][41].
* [Glade][328] - A RAD tool to enable quick development of GTK+
  GUIs. [GPL-2.0][8].
* [GMSL][331] - GNU Make Standard Library; a collection of additional
  functionality for GNU Make. [BSD-3-Clause][6].
* [GNU Global][330] - A source code tagging tool. [GPL-3.0][41].
* [GPP][269] - A general-purpose preprocessor. More versatile than the C
  preprocessor, but more flexible than m4. [LGPL-3.0+][5].
* [Highlight][333] - Converts source code to formatted text with nice
  highlighting. [GPL-3.0][41].
* [include-what-you-use][289] - Helps find unecessary inclusions and make
  suggestions for fixing them. Based on LLVM/Clang (and only works with
  it). [NCSA][39].
* [indent][315] - Formats C source code automatically to make it easier to
  read. Also converts from one style of source to another. [GPL-3.0+][41].
* [qo][274] - A build system that works without a separate config file. [MIT][11].
* [SMACK][500] - A modular software verification toolchain and a self-contained
  software verifier. Currently only works with programs compiled using Clang.
  [MIT][11].
* [unifdef][290] - Removes #ifdef and #if directives with their delimited text
  without touching any other part of the file. [BSD-3-Clause][6] or [BSD-2-Clause][24].

## Utilities ##

This is a 'catch-all' category for anything that doesn't fit well anywhere else.

* [ApeTagLibs][345] - A library for working with APEv2 tags. [MIT][11].
* [argparse][413] - A command-line argument parsing library, inspired by
  Python's argparse module. [MIT][11].
* [attr][425] - Commands for manipulating filesystem extended
  attributes. [GPL-2.0+][8].
* [bfd][157] - A library for manipulating binary object files. Part of GNU
  binutils. [GPL-3.0+][41].
* [Caffeine][496] - A library for building daemons and services for Linux and
  FreeBSD systems. [LGPL-2.1+][15].
* [CException][298] - An implementation of exceptions. [MIT][11].
* [CommonMark][223] - An implementation of the CommonMark spec. 
  [Variety of licenses, all free][224].
* [CRIU][440] - Checkpoint/Restore In Userspace; a software tool (with a C API)
  for 'freezing' a running application to disk, then restoring
  it. [GPL-2.0][8] or [LGPL-2.1][15].
* [D-Bus][430] - A simple way for applications to talk to one
  another. [AFL-2.1][431] or [GPL-2.0+][8].
* [Discount][438] - A simple implementation of a Markdown parser. [BSD-3-Clause][6].
* [dlx][388] - An implementation of [Knuth's Algorithm X][389], with example
  solvers. [GPL-3.0+][41].
* [docopt.c][270] - An implementation of a command-line option parser. [MIT][11].
* [dyncall][281] - Another foreign function interface library. [MIT][11].
* [Firm][361] - A library that provides a graph-based intermediate
  representation, optimizations and assembly code generation suitable for use in
  compilers. Comes with an example C front-end under the same
  license. [LGPL-2.1][15].
* [gjrand][327] - A library of random-number generation
  routines. [GPL-2.0][8] or [GPL-3.0][41].
* [GNU FreeIPMI][158] - An in-band and out-of-band IPMI
  implementation. [GPL-3.0][41].
* [GNU gperf][351] - A perfect hash function generator, given a list of
  strings. Outputs C code. [GPL-3.0+][41].
* [GNU Libffcall][162] - A collection of libraries for building foreign function
  interfaces. [GPL-3.0+][41].
* [Hoedown][405] - A fully-standards-compliant, extension-supporting, UTF-8
  aware, fast Markdown parser. [MIT][11].
* [iniparser][336] - A parser for .ini files. [MIT][11].
* [jwHash][350] - A fast hashtable implementation. [Apache-2.0][32].
* [kdtree][337] - A simple library for working with KD-trees. [BSD-3-Clause][6].
* [Kitsune][355] - An efficient, general-purpose framework for dynamic software
  updating. [LGPL-3.0+][5].
* [libavl][156] - A library containing a range of self-balancing binary
  trees. [GPL-3.0+][41].
* [libbson][235] - A BSON utility library. [Apache-2.0][32].
* [libCello][96] - A library introducing higher-level programming to
  C. [BSD-3-Clause][6].
* [libcmark][436] - A library for parsing the CommonMark dialect of
  Markdown. [BSD-2-Clause][24].
* [libcoap][136] - An implementation of the [Constrained Application Protocol][117].
  [GPL-2.0+][8] or [BSD-2-Clause][24].
* [libconfuse][135] - A small configuration file parser library. [ISC][61].
* [libcox][373] - A library which permits cross-platform system calls and
  standard utilities across different operating systems. [BSD-2-Clause][24].
* [libcsv][387] - A simple, streaming CSV parser. [LGPL-2.1+][15].
* [libffi][128] - A portable foreign-function interface library. [MIT][11].
* [libgeohash][499] - A pure C implementation of the Geohash algorithm.
  [BSD-3-Clause][6].
* [libgit2][108] - Pure C implementation of Git. [GPL-2.0, with a linking exception][109].
* [libgss][161] - Generic Security Service. [GPL-3.0+][41].
* [liblfds][411] - A portable lock-free data structure library. Public domain
  (more exactly, whatever license you want).
* [libimobiledevice][354] - A cross-platform protocol library to communicate
  with iThings. [LGPL-2.1+][15].
* [libnfc][332] - A platform-independent Near-Field Communication
  library. [LGPL-3.0][5].
* [libPhenom][31] - An eventing framework for building high-scalability and
  high-performance systems. [Apache-2.0][32].
* [libpostal][434] - A library for parsing and normalization of street addresses
  around the world. Powered by statistical NLP and open geo data. [MIT][11].
* [libtrading][455] - An implementation of network protocols for communicating
  with exchanges, dark pools and other trading venues. Supports FIX, FIX/FAST
  and many proprietary protocols. [BSD-2-Clause][24].
* [libucl][239] - A universal configuration library parser. [BSD-2-Clause][24].
* [libuv][56] - Cross-platform asynchronous I/O. [MIT][11].
* [libYAML][341] - A YAML 1.1 parser and emitter. [MIT][11].
* [libxo][407] - Allows an application to generate plain text, XML, JSON and
  HTML output using a common set of function calls. The application decides at
  runtime what output style should be produced. [BSD-2-Clause][24].
* [linenoise][504] - A small, self-contained alternative to readline and
  libedit. [BSD-2-Clause][24].
* [ncurses][178] - Coloured terminal UI library. [MIT][11].
* [netbsd-curses][494] - A simplified and small version of ncurses, with the same
  interface. [BSD-3-Clause][6].
* [nope.c][209] - An ultra-light software platform for scalable server-side and
  networking applications (think node.js for C programmers). [GPL-2.0][8].
* [pbc][236] - A protocol buffers library. [MIT][11].
* [progressbar][453] - An easy-to-use library for displaying text progress bars.
  [BSD-3-Clause][6].
* [rabbitmq-c][228] - A client library for [RabbitMQ][229]. [MIT][11].
* [Ragel][54] - A DSL for state machines that compiles to C. [GPL-2.0][8].
* [sort][190] - A collection of sorting routines, which type-specialize at
  compile-time with a user-defined type. [MIT][11].
* [termbox][396] - A library for writing text-based interfaces. [MIT][11].
* [tinyexpr][395] - A tiny recursive-descent parser, compiler and evaluation
  engine for simple mathematical expressions. [BSD-3-Clause][6].
* [Tulip Indicators][449] - A library of functions for technical analysis of
  financial data. [LGPL-3.0+][5].
* [vector.h][152] - A header library for typed lists. [MIT][11].
* [Viola][241] - A simplification of libCello. [MIT][11].
* [XLSX I/O][344] - A cross-platform library for reading and writing .xlsx
  files. [MIT][11].
* [zlog][437] - A reliable, pure C logging library. [LGPL-2.1][15].
* [zproto][421] - A protocol framework for ZeroMQ. [MIT][11].

## Windows Environments ##

This is a list of technologies designed to bring Windows into the 21st century
with respect to support for C.

* [Cygwin][253] - Designed to emulate a POSIX-compatible environment extensively
  under Windows. [Various licenses, all free][254].
* [MinGW-w64][287] - A minimalist environment for C development on Windows with
  64 bit support. [Various licenses, all free][252].
* [MSYS2][428] - Minimal SYStem 2; aims to provide support for a POSIX
  environment on Windows, with a package manager based on Arch Linux's
  pacman. Packages have individual licenses, otherwise, as MinGW and Cygwin.

## XML ##

> "XML is crap. Really. There are no excuses. XML is nasty to parse for humans,
> and it's a disaster to parse even for computers. There's just no reason for
> that horrible crap to exist." - Linus Torvalds

* [Expat][89] - A stream-oriented XML parser. [MIT][11].
* [libxml2][62] - A standards-compliant, portable XML parser. [MIT][11].

[1]: https://wiki.gnome.org/Projects/GLib
[2]: https://developer.gnome.org/gio/
[3]: https://developer.gnome.org/gobject/stable/
[4]: https://github.com/android/platform_bionic
[5]: https://spdx.org/licenses/LGPL-3.0.html
[6]: https://spdx.org/licenses/BSD-3-Clause.html
[7]: https://en.wikipedia.org/wiki/The_C_Programming_Language
[8]: https://spdx.org/licenses/GPL-2.0.html 
[9]: https://www.fefe.de/dietlibc/
[10]: https://www.musl-libc.org/
[11]: https://spdx.org/licenses/MIT.html
[12]: https://en.wikipedia.org/wiki/Widget_toolkit
[13]: https://en.wikipedia.org/wiki/Free_software
[14]: https://www.gtk.org/
[15]: https://spdx.org/licenses/LGPL-2.1.html
[16]: http://webserver2.tecgraf.puc-rio.br/iup/
[17]: https://github.com/saitoha/libsixel
[18]: https://www.enlightenment.org?p=about%252Flibs
[19]: http://www.tcl.tk/
[20]: https://spdx.org/licenses/TCL.html
[21]: http://xforms-toolkit.org/
[22]: https://www.sqlite.org/
[23]: https://unqlite.org/
[24]: https://spdx.org/licenses/BSD-2-Clause.html
[25]: https://mariadb.com/
[26]: https://github.com/clibs/clib
[27]: https://github.com/clibs/clib/wiki/Packages
[28]: http://www.koanlogic.com/libu/
[29]: https://github.com/antirez/sds
[30]: http://sglib.sourceforge.net/
[31]: http://facebook.github.io/libphenom/index.html
[32]: https://spdx.org/licenses/Apache-2.0.html
[33]: https://www.codeproject.com/Articles/6154/Writing-Efficient-C-and-C-Code-Optimization
[34]: http://re2c.org/index.html
[35]: http://shop.oreilly.com/product/0636920033677.do
[36]: http://shop.oreilly.com/product/0636920028000.do
[37]: http://www.openmp.org/
[38]: https://clang.llvm.org/
[39]: https://spdx.org/licenses/NCSA.html
[40]: https://gcc.gnu.org/
[41]: https://spdx.org/licenses/GPL-3.0.html
[42]: http://anjuta.org/
[43]: http://www.geany.org/
[44]: https://www.kdevelop.org/
[45]: https://www.codelite.org/
[46]: https://www.gnu.org/software/gnulib/
[47]: https://www.gnu.org/software/gsl/
[48]: http://liballeg.org
[49]: https://spdx.org/licenses/Zlib.html
[50]: https://www.libsdl.org/
[51]: https://redis.io/
[52]: http://zeromq.org/
[53]: http://www.digip.org/jansson/
[54]: http://www.colm.net/open-source/ragel/
[55]: http://dl.acm.org/citation.cfm?id=179241
[56]: https://github.com/libuv/libuv
[57]: https://www.gnu.org/software/libc/
[58]: https://github.com/silentbicycle/greatest
[59]: http://check.sourceforge.net/
[60]: https://lloyd.github.io/yajl/
[61]: https://spdx.org/licenses/ISC.html 
[62]: http://xmlsoft.org/
[63]: https://www.ffmpeg.org/
[64]: http://knking.com/books/c2/index.html
[65]: https://curl.haxx.se/libcurl/
[66]: https://spdx.org/licenses/curl.html
[67]: http://site.icu-project.org/
[68]: https://spdx.org/licenses/ICU.html 
[69]: http://lodev.org/lodepng/
[70]: http://www.fftw.org/
[71]: https://sourceforge.net/projects/kissfft/
[72]: https://bitbucket.org/MDukhan/yeppp
[73]: https://graphics.stanford.edu/~seander/bithacks.html
[74]: http://pcc.ludd.ltu.se/
[75]: http://pcc.ludd.ltu.se/licenses/
[76]: https://github.com/attractivechaos/klib
[77]: https://github.com/netmail-open/wjelement/
[78]: http://apr.apache.org/
[79]: https://gmplib.org/
[80]: https://github.com/cesanta/slre
[81]: http://tiny-rex.sourceforge.net/
[82]: https://github.com/laurikari/tre/
[83]: http://www.pcre.org/
[84]: https://github.com/Tuplanolla/cheat
[85]: http://www.valgrind.org/
[86]: https://www.gnu.org/software/binutils/
[87]: https://www.gnu.org/software/gdb/
[88]: https://github.com/fragglet/c-algorithms
[89]: http://expat.sourceforge.net/ 
[90]: https://www.sfml-dev.org/download/csfml/
[91]: https://www.sfml-dev.org/index.php
[92]: https://github.com/siu/minunit
[93]: https://github.com/keybuk/libnih
[94]: http://cunit.sourceforge.net/
[95]: http://rr-project.org/
[96]: http://libcello.org/
[97]: http://nethack4.org/projects/aimake/
[98]: http://www.glfw.org/
[99]: https://github.com/dcnieho/FreeGLUT
[100]: https://spdx.org/licenses/X11.html 
[101]: https://github.com/orangeduck/Corange
[102]: http://shop.oreilly.com/product/0636920015482.do
[103]: http://ccodearchive.net/
[104]: http://ccodearchive.net/list.html
[105]: https://symas.com/lightning-memory-mapped-database/
[106]: https://spdx.org/licenses/OLDAP-2.8.html
[107]: https://github.com/ioquake/ioq3
[108]: https://libgit2.github.com/
[109]: https://github.com/libgit2/libgit2/blob/master/COPYING
[110]: https://www.openssl.org/
[111]: https://www.openssl.org/source/license.html
[112]: http://www.gnutls.org/
[113]: https://github.com/RhysU/c99sh
[114]: https://github.com/nothings/stb
[115]: https://tinycthread.github.io/
[116]: http://bstring.sourceforge.net/
[117]: http://coap.technology/
[118]: http://facil.io/
[119]: https://www.enlightenment.org?p=about%252Fefl
[120]: http://zserge.com/jsmn.html
[121]: https://www.postgresql.org/
[122]: https://spdx.org/licenses/PostgreSQL.html 
[123]: https://gstreamer.freedesktop.org/
[124]: http://libevent.org/
[125]: https://www.hboehm.info/gc/
[126]: https://blogs.gnome.org/clutter/get-it/
[127]: https://github.com/rib/cogl-web/wiki
[128]: https://github.com/atgreen/libffi
[129]: https://github.com/protobuf-c/protobuf-c
[130]: https://github.com/jmckaskill/c-capnproto
[131]: https://en.wikipedia.org/wiki/External_Data_Representation
[132]: https://bitbucket.org/martijnj/msgpackalt
[133]: http://www.netlib.org/lapack/lapacke.html
[134]: http://www.netlib.org/lapack/
[135]: https://github.com/martinh/libconfuse
[136]: https://github.com/obgm/libcoap 
[137]: http://math-atlas.sourceforge.net/
[138]: http://lionet.info/asn1c/compiler.html
[139]: https://github.com/nanomsg/nanomsg
[140]: http://avro.apache.org/docs/current/api/c/index.html#_introduction_to_avro_c
[141]: https://cmocka.org/
[142]: https://www.gnu.org/software/libgcrypt/
[143]: https://github.com/libressl-portable/
[144]: http://software.schmorp.de/pkg/libev.html
[145]: https://google.github.io/flatbuffers/
[146]: https://en.wikipedia.org/wiki/POSIX_Threads
[147]: https://www.opengl.org/
[148]: http://www.sgi.com/tech/opengl/?/license.html
[149]: https://github.com/flycheck/flycheck
[150]: http://joaotavora.github.io/yasnippet/
[151]: http://valloric.github.io/YouCompleteMe/
[152]: https://sites.google.com/site/lccretargetablecompiler/
[153]: https://github.com/drh/lcc/blob/master/CPYRIGHT
[152]: https://github.com/swenson/vector.h
[155]: https://www.gnu.org/software/adns/
[156]: http://adtinfo.org/libavl.html/index.html
[157]: http://sourceware.org/binutils/docs/bfd/
[158]: https://gnu.org/software/freeipmi/index.html
[159]: https://gnu.org/software/glpk/
[160]: https://gnu.org/software/gsasl/
[161]: https://gnu.org/software/gss/
[162]: https://gnu.org/software/libffcall/
[163]: https://gnu.org/software/libiconv/
[164]: https://gnu.org/software/libidn/
[165]: https://gnu.org/software/libmicrohttpd/
[166]: http://www.hughes.com.au/products/libhttpd/
[167]: https://wiki.gnome.org/action/show/Projects/libsoup?action=show&redirect=LibSoup
[168]: http://www.webdav.org/neon/
[169]: http://mihl.sourceforge.net/
[170]: https://www.coralbits.com/libonion/
[171]: https://docs.cesanta.com/mongoose/master/
[172]: https://gnu.org/software/libtool/
[173]: https://gnu.org/software/libunistring/
[174]: https://gnu.org/software/libxmi/
[175]: http://www.multiprecision.org/index.php?prog=mpc&page=home
[176]: http://mpfr.loria.fr/index.html
[177]: https://gnu.org/software/mpria/
[178]: https://gnu.org/software/ncurses/
[179]: https://gnu.org/software/osip/
[180]: https://gnu.org/software/pth/
[181]: http://careferencemanual.com/
[182]: http://shop.oreilly.com/product/9780596004361.do
[183]: http://shop.oreilly.com/product/0636920026136.do
[184]: https://www.pearsonhighered.com/program/Prata-C-Primer-Plus-6th-Edition/PGM4399.html
[185]: http://www.planetpdf.com/codecuts/pdfs/ooc.pdf
[186]: https://github.com/vim-syntastic/syntastic
[187]: https://github.com/dvidelabs/flatcc
[188]: https://github.com/b-k/apophenia
[189]: https://github.com/b-k/apophenia/blob/master/install/COPYING
[190]: https://github.com/swenson/sort
[191]: http://steve-yegge.blogspot.co.nz/2008/10/universal-design-pattern.html
[192]: http://libjpeg.sourceforge.net/
[193]: http://libjpeg-turbo.virtualgl.org/
[194]: http://www.libjpeg-turbo.org/About/License
[195]: https://github.com/liuliu/ccv
[196]: https://github.com/google/gumbo-parser
[197]: https://github.com/joyent/http-parser
[198]: https://github.com/jedisct1/libsodium
[199]: https://github.com/lpereira/lwan
[200]: https://github.com/mozilla/mozjpeg
[201]: https://github.com/redis/hiredis
[202]: http://jvns.ca/blog/2014/12/14/fun-with-threads/
[203]: https://github.com/silentbicycle/socket99
[204]: http://danluu.com/malloc-tutorial/
[205]: http://www.tedunangst.com/flak/post/memcpy-vs-memmove
[206]: https://blogs.oracle.com/ksplice/entry/8_gdb_tricks_you_should
[207]: https://www.youtube.com/playlist?list=PLLX-Q6B8xqZ8n8bwjGdzBJ25X2utwnoEG
[208]: http://nethack4.org/blog/building-c.html
[209]: https://github.com/riolet/WAFer
[210]: https://docs.google.com/presentation/d/1h49gY3TSiayLMXYmRMaAEMl05FaJ-Z6jDOWOz3EsqqQ/edit?pli=1#slide=id.gaf50702c_0153
[211]: http://cppinstitute.com/study-resources
[212]: http://www.crasseux.com/books/ctut.pdf
[213]: http://home.netcom.com/~tjensen/ptr/pointers.htm
[214]: https://github.com/adamierymenko/huffandpuff
[215]: https://sourceforge.net/projects/vtd-xml/
[216]: http://www.msweet.org/projects.php?Z3
[217]: http://svn.msweet.org/mxml/trunk/COPYING
[218]: http://ezxml.sourceforge.net/
[219]: https://github.com/blunderer/libroxml
[220]: https://github.com/json-c/json-c/wiki
[221]: https://github.com/id-Software/Quake-2
[222]: https://github.com/dinhviethoa/libetpan
[223]: https://github.com/jgm/CommonMark
[224]: https://github.com/jgm/CommonMark/blob/master/LICENSE
[225]: https://github.com/id-Software/Quake
[226]: https://github.com/zeromq/czmq
[227]: https://spdx.org/licenses/MPL-2.0.html
[228]: https://github.com/alanxz/rabbitmq-c
[229]: http://www.rabbitmq.com/
[230]: https://github.com/madler/zlib
[231]: https://github.com/libretro/RetroArch
[232]: https://www.libretro.com/
[233]: http://mongoc.org/
[234]: https://www.mongodb.org/
[235]: https://github.com/mongodb/libbson
[236]: https://github.com/cloudwu/pbc
[237]: https://github.com/sinemetu1/twitc
[238]: https://github.com/orangeduck/mpc
[239]: https://github.com/vstakhov/libucl
[240]: http://snaipe.me/c/c-smart-pointers/
[241]: https://github.com/eatonphil/Viola
[242]: https://github.com/concurrencykit/ck
[243]: http://repo.hu/projects/cchan/
[244]: https://github.com/pmwkaa/sophia
[245]: http://www.greenend.org.uk/rjk/tech/inline.html
[246]: https://github.com/Snaipe/Criterion
[247]: http://www.open-std.org/JTC1/SC22/WG14/
[248]: https://en.wikibooks.org/wiki/C_Programming
[249]: http://www.codeblocks.org/
[250]: http://cedet.sourceforge.net/
[251]: http://mingw.org/
[252]: http://mingw.org/license
[253]: https://cygwin.com/
[254]: https://cygwin.com/licensing.html
[255]: http://flintlib.org/
[256]: http://pari.math.u-bordeaux.fr/
[257]: http://blog.noctua-software.com/c-tricks.html
[258]: http://www.eclipse.org/ide/
[259]: https://spdx.org/licenses/EPL-1.0.html
[260]: https://netbeans.org/
[261]: https://github.com/JonnyWhatshisface/libwebsock
[262]: http://c-faq.com/
[263]: https://computing.llnl.gov/tutorials/pthreads/
[264]: https://computing.llnl.gov/tutorials/openMP/
[265]: https://computing.llnl.gov/tutorials/mpi/
[266]: https://www.securecoding.cert.org/confluence/display/c/SEI+CERT+C+Coding+Standard
[267]: http://blog.pkh.me/p/20-templating-in-c.html
[268]: http://lipforge.ens-lyon.fr/www/crlibm/index.html
[269]: https://logological.org/gpp
[270]: https://github.com/docopt/docopt.c
[271]: http://marek.vavrusa.com/c/memory/2015/02/20/memory/
[272]: http://kukuruku.co/hub/programming/i-do-not-know-c
[273]: http://kamalatta.ddnss.de/otherdocs/pikestyle.html
[274]: https://github.com/andlabs/qo
[275]: http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html
[276]: https://github.com/ryanmjacobs/c
[277]: https://github.com/wolkykim/qlibc
[278]: https://github.com/wolkykim/qlibc/blob/master/LICENSE
[279]: https://gist.github.com/eatonphil/21b3d6569f24ad164365
[280]: https://www.flourish.org/cinclude2dot/
[281]: http://www.dyncall.org/
[282]: http://www.mcs.anl.gov/petsc/
[283]: http://slepc.upv.es/
[284]: https://github.com/open-mpi/ompi
[285]: http://www.mpich.org/
[286]: http://git.mpich.org/mpich.git/blob_plain/6aab201f58d71fc97f2c044d250389ba86ac1e3c:/COPYRIGHT
[287]: http://mingw-w64.yaxm.org/doku.php/start
[288]: https://github.com/google/sanitizers
[289]: https://github.com/include-what-you-use/include-what-you-use
[290]: http://dotat.at/prog/unifdef/
[291]: https://tls.mbed.org/
[292]: http://www.fefe.de/djb/
[293]: http://www.canonware.com/jemalloc/
[295]: https://github.com/gperftools/gperftools
[296]: https://github.com/ThrowTheSwitch/Unity
[297]: https://github.com/ThrowTheSwitch/CMock
[298]: https://github.com/ThrowTheSwitch/CException
[299]: https://github.com/libtom/libtomcrypt
[300]: https://pngquant.org/lib/
[301]: https://wiki.haskell.org/Introduction_to_QuickCheck2
[302]: https://github.com/silentbicycle/theft
[303]: https://github.com/slembcke/Chipmunk2D
[304]: https://biicode.github.io/biicode/
[305]: https://www.gnu.org/software/autoconf/
[306]: https://www.gnu.org/software/automake/automake.html
[307]: https://www.gnu.org/software/complexity/
[308]: http://www.eso.org/sci/software/cpl/
[309]: http://www.cprover.org/cbmc/
[310]: https://spdx.org/licenses/BSD-4-Clause.html
[311]: https://fakenmc.github.io/cf4ocl/
[312]: https://www.khronos.org/opencl/
[313]: http://c2html.sourceforge.net/whatisc2html.html
[314]: http://astyle.sourceforge.net/
[315]: https://www.gnu.org/software/indent/
[316]: http://www.feynarts.de/cuba/
[317]: http://www.gedanken.org.uk/software/cxref/
[318]: http://www.stack.nl/~dimitri/doxygen/index.html
[319]: https://www.gtk.org/gtk-doc/
[320]: https://www.gnu.org/software/ddd/ddd.html
[321]: http://docutils.sourceforge.net/
[322]: https://hplgit.github.io/doconce/doc/web/index.html
[323]: http://fabutil.org/
[324]: https://www.gnu.org/software/make/
[325]: http://leenissen.dk/fann/wp/
[326]: http://gittup.org/tup/index.html
[327]: https://sourceforge.net/projects/gjrand/
[328]: https://glade.gnome.org/
[329]: https://www.gnu.org/software/gnu-c-manual/
[330]: https://www.gnu.org/software/global/
[331]: http://gmsl.sourceforge.net/
[332]: https://github.com/nfc-tools/libnfc
[333]: http://www.andre-simon.de/index.php
[334]: https://spdx.org/licenses/LGPL-2.0.html 
[335]: https://spdx.org/licenses/GPL-1.0.html 
[336]: https://github.com/ndevilla/iniparser
[337]: https://github.com/jtsiomb/kdtree
[338]: http://www.oberhumer.com/opensource/lzo/
[339]: http://www.nlnetlabs.nl/projects/ldns/index.html
[340]: https://wiki.gnome.org/Projects/LibRsvg
[341]: http://www.pyyaml.org/wiki/LibYAML
[342]: https://www.xiph.org/ao/
[343]: http://www.chiark.greenend.org.uk/~sgtatham/mp/
[344]: https://brechtsanders.github.io/xlsxio/
[345]: https://github.com/jeremyevans/ape_tag_libs/tree/master/c
[346]: http://www.mission-base.com/peter/source/
[347]: http://cdecl.org/
[348]: https://github.com/mpv-player/mpv
[349]: https://www.recurse.com/blog/5-learning-c-with-gdb
[350]: https://github.com/watmough/jwHash
[351]: https://www.gnu.org/software/gperf/
[352]: http://libmill.org/
[353]: https://talloc.samba.org/talloc/doc/html/index.html
[354]: https://github.com/libimobiledevice/libimobiledevice
[355]: http://kitsune-dsu.com/
[356]: https://github.com/abiggerhammer/hammer
[357]: http://250bpm.com/blog:56
[358]: http://www.samnip.ps/thought/macro-storage-for-inverse-comma
[359]: https://github.com/awslabs/s2n
[360]: https://www.gnu.org/software/recutils/
[361]: http://pp.ipd.kit.edu/firm/
[362]: http://www.etalabs.net/compare_libcs.html
[363]: https://github.com/Ed-von-Schleck/shoco
[364]: https://github.com/antirez/smaz
[365]: https://github.com/prideout/heman
[366]: https://github.com/cacalabs/libcaca
[367]: https://spdx.org/licenses/WTFPL.html 
[368]: http://mesonbuild.com/
[369]: https://icculus.org/twilight/darkplaces/
[370]: https://bitbucket.org/orx/orx
[371]: https://github.com/zturtleman/spearmint
[372]: https://github.com/andrewrk/libsoundio
[373]: http://libcox.symisc.net/
[374]: http://proprogramming.org/some-unknown-features-or-tricks-in-c-language/
[375]: https://perf.wiki.kernel.org/index.php/Main_Page 
[376]: https://github.com/timonwong/libao
[377]: https://github.com/camgunz/cmp
[378]: https://github.com/ludocode/mpack
[379]: http://msgpack.org/
[380]: http://www.oracle.com/us/products/database/berkeley-db/overview/index.html
[381]: https://spdx.org/licenses/AGPL-1.0.html 
[382]: http://www.libpng.org/
[383]: https://spdx.org/licenses/Libpng.html
[384]: http://cairographics.org/
[385]: https://spdx.org/licenses/MPL-1.1.html 
[386]: https://github.com/balde/balde
[387]: http://sourceforge.net/projects/libcsv/
[388]: https://github.com/blynn/dlx
[389]: https://en.wikipedia.org/wiki/Knuth's_Algorithm_X
[390]: https://github.com/sharow/libconcurrent
[391]: https://hintjens.gitbooks.io/scalable-c/content/index.html
[392]: https://github.com/nemequ/munit/
[393]: https://github.com/quixdb/squash
[394]: https://github.com/codeplea/minctest
[395]: https://github.com/codeplea/tinyexpr
[396]: https://github.com/nsf/termbox
[397]: http://opic.rocks/
[398]: https://github.com/waruqi/tbox
[399]: http://sourceforge.net/projects/libquickmail/
[400]: https://github.com/liteserver/binn
[401]: https://sourceforge.net/projects/giflib/
[402]: https://github.com/libgd/libgd
[403]: https://embed.cs.utah.edu/creduce/
[404]: http://www.gnu.org/software/cflow/
[405]: https://github.com/hoedown/hoedown
[406]: https://github.com/srdja/Collections-C
[407]: https://github.com/Juniper/libxo
[408]: https://github.com/vurtun/nuklear
[409]: https://github.com/blunderer/libroxml
[410]: http://www.spinellis.gr/cscout/
[411]: http://liblfds.org/
[412]: https://github.com/codeplea/genann
[413]: https://github.com/cofyc/argparse
[414]: https://github.com/anholt/libepoxy
[415]: https://kore.io/
[416]: http://zeromq.org/
[417]: https://wiki.gnome.org/action/show/Projects/LibRsvg?action=show&redirect=LibRsvg
[418]: http://shop.oreilly.com/product/0636920033844.do
[419]: https://github.com/zeromq/zyre
[420]: https://github.com/zeromq/zproject
[421]: https://github.com/zeromq/zproto
[422]: https://github.com/it4e/CHL
[423]: http://www.koanlogic.com/klone/
[425]: http://savannah.nongnu.org/projects/attr/
[426]: https://sourceforge.net/projects/tinyfiledialogs/
[427]: http://www.bzip.org/
[428]: http://msys2.github.io/
[429]: http://www.libsigil.com/
[430]: https://www.freedesktop.org/wiki/Software/dbus/
[431]: https://spdx.org/licenses/AFL-2.1.html 
[432]: http://lzip.nongnu.org/clzip.html
[433]: http://lzip.nongnu.org/lzip.html
[434]: https://github.com/openvenues/libpostal
[435]: https://github.com/premake/premake-core
[436]: https://github.com/jgm/cmark
[437]: http://hardysimpson.github.io/zlog/
[438]: http://www.pell.portland.or.us/~orc/Code/discount/
[439]: https://github.com/clMathLibraries/clBLAS
[440]: https://criu.org/Main_Page
[441]: https://github.com/neomake/neomake
[442]: http://libdill.org/
[443]: https://github.com/DaveGamble/cJSON
[444]: https://github.com/ands/lightmapper
[445]: http://blosc.org/
[446]: https://github.com/Kazade/kazmath
[447]: http://pdclib.e43.eu/
[448]: https://creativecommons.org/publicdomain/zero/1.0/
[449]: https://tulipindicators.org/
[450]: https://locklessinc.com/benchmarks_allocator.shtml
[451]: https://locklessinc.com/
[452]: https://github.com/distcc/distcc
[453]: https://github.com/doches/progressbar
[454]: http://mpitutorial.com/
[455]: http://libtrading.org/
[456]: https://github.com/prideout/par
[457]: https://github.com/grimfang4/sdl-gpu
[458]: http://www.mega-nerd.com/libsndfile/
[459]: https://github.com/parallella/pal
[460]: https://tatsuhiro-t.github.io/wslay/
[461]: http://www.libtom.net/LibTomMath/
[462]: http://www.libtom.net/TomsFastMath/
[463]: http://www.libtom.net/LibTomPoly/
[464]: https://github.com/LibVNC/libvncserver
[465]: https://github.com/yosefk/checkedthreads
[466]: https://ccache.samba.org/
[467]: https://github.com/esneider/debug
[468]: https://lldb.llvm.org/
[469]: https://github.com/JuliaLang/utf8proc
[470]: https://github.com/vmg/clar
[471]: https://github.com/powturbo/TurboPFor
[472]: https://github.com/sheredom/utf8.h
[473]: https://github.com/troydhanson/tpl
[474]: http://liburcu.org/
[475]: http://oprofile.sourceforge.net/news/
[476]: http://libcork.readthedocs.io/en/0.14.0/
[477]: https://github.com/bashrc/libdeep
[478]: https://github.com/xant/libhl
[479]: https://github.com/josephg/librope
[480]: https://github.com/miracl/MIRACL
[481]: https://github.com/RoaringBitmap/CRoaring
[482]: http://roaringbitmap.org/
[483]: https://github.com/cvxgrp/scs
[484]: https://github.com/powturbo/TurboRLE
[485]: https://github.com/trezor/trezor-crypto
[486]: https://github.com/NuxiNL/cloudlibc
[487]: https://en.wikipedia.org/wiki/Capability-based_security
[488]: https://github.com/NeonMercury/jfes
[489]: https://en.wikipedia.org/wiki/Lexical_analysis
[490]: https://en.wikipedia.org/wiki/Parsing
[491]: https://github.com/westes/flex
[492]: https://www.gnu.org/software/bison/
[493]: https://openquantumsafe.org/
[494]: https://github.com/sabotage-linux/netbsd-curses
[495]: https://github.com/lemire/clhash
[496]: https://github.com/dmw/caffeine
[497]: https://github.com/fredrik-johansson/arb
[498]: https://github.com/theck01/offbrand_lib
[499]: https://github.com/simplegeo/libgeohash
[500]: https://github.com/smackers/smack
[501]: http://cppcheck.sourceforge.net/
[502]: https://clang.llvm.org/docs/ClangCheck.html
[503]: https://github.com/bvdberg/ctest
[504]: https://github.com/antirez/linenoise
[505]: https://github.com/memononen/nanovg
[506]: https://github.com/centaurean/density
[507]: http://maciejczyzewski.me/retter/
[508]: http://lz4.github.io/lz4/
[509]: https://github.com/spotify/sparkey
[510]: http://facebook.github.io/zstd/
[511]: http://www.vips.ecs.soton.ac.uk/index.php?title=VIPS
[512]: http://whitedb.org/
[513]: http://paulbatchelor.github.io/proj/soundpipe.html
[514]: https://github.com/atomicobject/heatshrink
[515]: http://ebassi.github.io/graphene/
[516]: https://github.com/raysan5/raylib
[517]: https://github.com/kkos/oniguruma
[518]: https://github.com/k-takata/Onigmo
[519]: https://github.com/lemire/simdcomp
[520]: https://github.com/kuba--/zip
[521]: https://spdx.org/licenses/Unlicense.html
[522]: https://github.com/Cyan4973/xxHash
[523]: https://github.com/aubio/aubio
[524]: https://github.com/groonga/groonga
[525]: https://github.com/100/Cranium
[526]: http://www.saphir2.com/sphlib/
[527]: https://github.com/google/highwayhash
[528]: http://nullprogram.com/blog/2017/08/20/
[529]: http://nullprogram.com/blog/2017/09/21/
[530]: https://graphics.stanford.edu/~seander/bithacks.html
