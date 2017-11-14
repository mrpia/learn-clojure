# learn-clojure

Resources I've found helpful on my journey learning Clojure.

Most if not all of the credit goes to my Clojure mentor & work colleague [Jonas Emanuel Müller](mailto:jonas.mueller@gmail.com), whose digital live can be observed at [jonasmueller.net](https://jonasmueller.net/). What started as fascinating lunch discussions and slack conversations turned into this. Thanks mate for challenging and guiding me on the journey!

## Getting ready to learn Clojure

Don't start by learning Clojure. First **learn why you should learn Clojure**. At best with a lot of videos, so you can intensely absorb [Rich Hickey](https://twitter.com/richhickey)'s arguments while commuting.

Start with [Effective Programs - 10 Years of Clojure](https://www.youtube.com/watch?v=2V1FtfBDsLU), it tells you *why* the language exists and what its *goal* is: **productivity in the enterprise**. If you prefer reading, go for a [transcription](https://github.com/matthiasn/talk-transcripts/blob/master/Hickey_Rich/EffectivePrograms.md) (for some reason people love to transcribe Rich's talks). For more detailed explanations on *how* Clojure is better at achieving that goal than any other language you'll need to follow up with other talks.

A next great step is [Simple Made Easy](https://www.infoq.com/presentations/Simple-Made-Easy), it gives you insight into the central philosophy behind Clojure. Note how the talk isn't about Clojure, but about **how to be a better programmer/thinker in general**. Jonas has watched the talk many times and admitted he still learns new things every time. If you want some third party opinion on why your time isn't wasted with this talk you could for example have a look at this [Hacker News thread](https://news.ycombinator.com/item?id=4173854).

The last abstract talk Jonas strongly recommends is really important before going practical: [The Value of Values](https://www.infoq.com/presentations/Value-Values). Depending on your background, be prepared to be provoked a bit, since that's the part where Rich also criticises object-oriented programming. Luckily for me, Jonas thought I seemed *"very surprisingly open to these kinds of thoughts and ideas"*.

If you're eager for more, check out [Rich Hickey's greatest hits](https://changelog.com/posts/rich-hickeys-greatest-hits).

As one of the side-benefits of these talks, you get to learn funky new words, such as:

- [homoiconicity](https://en.wikipedia.org/wiki/Homoiconicity) indicates that a program's source code is written as a basic data structure that the programming language knows how to access, for more details read about [the Clojure Reader](https://clojure.org/reference/reader)
- [reification](http://www.lispcast.com/reification) means making an abstraction into a concrete value that can be manipulated at runtime.

Now you can impress your peers by combining these terms together, as Clojure's *homoiconicity* means that programs are *reified* into the language as *data*.

## Learning Clojure

Armed with all the theoretical motivation, I've decided to buy the excellent [Clojure for the Brave and True](https://www.braveclojure.com/clojure-for-the-brave-and-true/) book to guide me a bit more in my journey.

Do *not* try to understand the official Clojure documentation. Or at least not after a few years of Clojure practice ;) It's meant as a reference. Instead, use the community-driven [CDS Clojure Documentation](http://clojure-doc.org/)

The [Clojure Design Patterns](http://mishadoff.com/blog/clojure-design-patterns/) article is somewhat biased towards Clojure but it's still an interesting comparison of compactness between Clojure and Java.

For learning in the tram go with [4Clojure](http://www.4clojure.com/), a very popular way of learning Clojure, also available as mobile apps.

This [visual cheatsheet](https://s-haensch.github.io/visual-cheatsheet/) is also good for beginners.

Clojure makes users way more aware of data structures and their performance implications than many statically typed languages. For example one uses different functions to append to an array and a (linked) list, because one should be aware of the performance/computational complexity differences.

Learn [clojure.spec](https://clojure.org/about/spec) in due time. That is, only when you're comfortable reading and writing Clojure ;)

## Tools

The [Cursive IntelliJ IDEA plugin](https://cursive-ide.com/) proved ideal for the Jetbrains fan that I am. [This](https://cursive-ide.com/userguide/paredit.html) even shows you one of the reasons Lisp parentheses are awesome: you don't actually write/type them, you use them to manipulate your code semantically.

Some people prefer [Spacemacs](http://spacemacs.org/).

## Clojure vs the rest of the world

People on the outside seem more focused on the fact that Clojure is a Lisp than Clojurians are. Read: *"Oh no, parentheses-hell!"*. Among Clojurians it is common to hear *"I came for the Lisp, but I stayed for the immutability"*.

## Beyond Clojure

Rich Hickey & co think it's so important that data can be typed that created the [Transit](https://github.com/cognitect/transit-format) format, an extended version of JSON that has more types (so you can for example transmit dates properly!) and can be extended with more types. And they implemented libraries for the major languages.

If you think that *immutable data*, as well as *data as a first-class citizen of your end-to-end software world* are fantastic  concepts, then check out [Datomic](http://www.datomic.com/).
