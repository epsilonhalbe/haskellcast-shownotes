HC007 - Chris Done on Compiling to JavaScript and SQL
=====================================================

Intro
-----
- Chris Done [blog](http://chrisdone.com/) [@christopherdone](https://twitter.com/christopherdone)
- [C](http://en.wikipedia.org/wiki/C_programming_language)
- [Scheme](https://en.wikipedia.org/wiki/Scheme\_(programming\_language))
- [lambdas](https://en.wikipedia.org/wiki/Lambda\_calculus)
- [haskell implementation of scheme](http://jonathan.tang.name/files/scheme\_in\_48/tutorial/overview.html)
- [idris](http://www.idris-lang.org/)
- [lpaste](http://lpaste.net/) formerly known as hpaste
- [tryhaskell.org](http://tryhaskell.org/)
- [mueval](http://hackage.haskell.org/package/mueval) not related to
- [mu]() a spinoff language from haskell used at standard chartered
- [hint](http://hackage.haskell.org/package/hint) - safe evaluate haskell code *Author*: Daniel Gorin
- [FP Complete](https://www.fpcomplete.com/)
- [FP Haskell Center™](https://www.fpcomplete.com/business/haskell-center/overview/)
- [containers]()
- [Fay](http://Fay-lang.org/ )

History of Fay
--------------

- [GHCjs](https://github.com/GHCjs) (Luite Stegeman, Hamish Mackenzie)
- [UHC](https://github.com/UU-ComputerScience/uhc)
- [YHC](http://www.haskell.org/haskellwiki/Yhc)
- [AST](http://en.wikipedia.org/wiki/Abstract_syntax_tree)
- [haskell-src-exts](http://hackage.haskell.org/package/haskell-src-exts) (typeclasses)
- [haskell-names](http://hackage.haskell.org/package/haskell-names) (name resolution)
- FP Complete IDE - almost entirely written in Fay

Haskell to JavaScript transpilers
---------------------------------

### Fay
+ Output small
+ Simple
+ Haskell + [thunk](http://en.wikipedia.org/wiki/Thunk) & forcing wrappers
+ Small compiler
+ [Foreign Function Interface](http://en.wikipedia.org/wiki/Foreign_function_interface) (FFI) to js (jquery), callbacks, native types based on UHC's FFI
+ Convenient
+ No dependency on [GHC]()
- No typeclasses


### GHCJavaScript
+ Supports typeclasses
+ Full typechecking
+ Can compile Fay
+ Software Transactional Memory
  - [wiki|STM](http://en.wikipedia.org/wiki/Software_transactional_memory) (http://book.realworldhaskell.org/read/software-transactional-memory.html)
  - [rwh|STM](http://book.realworldhaskell.org/read/software-transactional-memory.html)
  - [pch|STM](http://chimera.labs.oreilly.com/books/1230000000929/ch10.html)
+ [Threads](http://en.wikipedia.org/wiki/Thread\_(computing))
+ Faster than Fay
- Large (used to be huge)
- Haskell FFI

### Haste
+ STG (see below )
+ Threads
+ Asynchronous (like JavaScript)
+ FFI like (UHC/Fay)
+ Hs98 + Exstensions
- GHC Runtime

GHC compiling steps
-------------------
- Haskell
- Core
- STG
- C--
- LLVM/ASM

Static typing for JavaScript
----------------------------

- [Typescript](http://www.typescriptlang.org/)
- [Purescript](http://functorial.com/purescript/)
- [Roy](http://roy.brianmckenna.org/)

- Overhead - Performance - Debugging

- [Segfault](https://en.wikipedia.org/wiki/Segmentation_fault)

- [Source maps](http://code.google.com/p/closure-compiler/wiki/SourceMaps) (help with debugging)?
- GHCi (+ debugging)
- Chris Forno - Fay videos [part1], [part2]

Compiling Haskell to JavaScript
-------------------------------

- [History of JavaScript](https://brendaneich.com/2010/07/a-brief-history-of-javascript/) (talk)
- Native client
- Virtual machine
- [AHC](https://github.com/strake/ahc)

- Adoption of Fay
- FP Haskell Center™ (15000 lines)
- Not so fast anymore
- [Adam Bergmark](https://github.com/bergmark)

Haskell & Modulesystem
----------------------

- [Gzip](www.gzip.org)
- [Closure](https://developers.google.com/closure/compiler/) (compiler)
- [Clojurescript](https://github.com/clojure/clojurescript)
- ACL

TryHaskell
===============

- [Tryruby](http://tryruby.org/) by \_y
- Lamdabot: [haskellWiki](http://www.haskell.org/haskellwiki/Lambdabot),[hackage](http://hackage.haskell.org/package/lambdabot)
- [Try Clojure](http://tryclj.com/)
- [Tryarc](http://tryarc.org/)
- [Try Git](https://try.github.io/)
- Remote code evaluation - malicious attacks
- Mueval
- [Common lisp](https://en.wikipedia.org/wiki/Common_Lisp)
- [Sandbox](https://en.wikipedia.org/wiki/Sandbox\_(computer\_security))
- Impure io


- Pure io (blog)
- Free monad
- Russel o'connor (free monad implementation)
- Laws (monad laws)

How does Chris Done learn new
------------------------------
- Free monads - Gabriel Gonzalez' tutorials
- Tutorials
- GHCi + :t,:k

> Connor McBride: "types should guide, not slap you on the wrist"

### Funky functions?

- Add function parameters until kind = *
- Polymorphism
- Arrow
- Hakyll
- Jasper van der euicht
- Bimap
- Bifunctor

- Web development

Haskelldb
---------

- Databases

- Combinators
- Select/Restrict/Project
- HList
- SQL
- Type level programming (blog)
- Monad for composition - pagination

- Active record
- ORM
- LINQ

- Relation database - original paper??

Rein Henrichs on Ruby
----------------------

- Algebra
- Relational algebra
- Asymptotic
- Caching
- Cache evacuation
- Arel

Haskell DB - again
-----------------

- Haskell DB does not optimize queries
- PostgreSQL

- Optimization
- Plated
- Lens
- Term replacement
- Uniplate
- Traverse
- Fixpoint

- Equelito
- Persistent (no joins)
- Custom queries

Hell - haskell shell
--------------------

###How to launch program

1. name bind program
2. string -> system
3. all of `/usr/bin/` -> bind in scope

Shell scripting
---------------

- Bash
- Cabal
- Shebang
- Dbus
- Pipes (bash)
- Pipes/ conduit
- Tail f > grep
- Shell based on pipes (gabriel)
- Shelly
- Reader monad

Hulk - irc server
-----------------

- Sockets connections threads
- MVar
- Resource handling

Emacs
=====

- Structured haskell mode
- Vim
- Evil mode
- God mode
- Rsi
- Lambdu
- Minor mode
- Semantic editing
- Haskell-src-exts
- Vimscript
- Elisp
- Cpp-lines
- Chris Done on Youtube
- More haskell videos
- Chris Forno - announces Emacs video

Shoutouts - stuff to mention
----------------------------

- Logic language - parsed with attempto controled english
- Datalog
- Interactive book

- Stackage (blog) to come
- Loeb

Question
========

If you take a möbius strip cut along the center line what do you get?

1. 2 Möbius stip
2. 1 Möbius stip
3. 1 Tangled not möbius strip


[part1]: http://www.youtube.com/watch?v=hS52OdD6mdo
[part2]: http://www.youtube.com/watch?v=PnMxT3cjYt8
