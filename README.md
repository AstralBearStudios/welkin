
# Table of Contents


⚠ **\*Warning: This repository is a WIP. This project is in its early stages and does not have any code. Please wait to submit any issues, and stay tuned for updates.**

**Major Update, February 27, 2024** I have realized that the Standard and initial implementation aimed to do too much and had scope creep. I realized that welkin does not need to do everything in one go and emphasize how it is a *universal information format.* This means two big things for the project:

- The Standard will prioritize on one task: *formally specify* the Welkin language:
    - Syntax: Has a precise LALR grammar, with details on every terminal and rules.    - Semantics: Defines a WIG (Welkin Information Graph) and its notion of equivalence.
Every possible detail will be considered, in order to avoid ambiguities in other formats (including JSON). In order to simplify things and avoid confusion, there will no longer be any variants: there will be *exactly one grammar* and semantics to refer to. Because Welkin is contained, *the Welkin interpreter will not be specified.* Instead, *the interpreter's specification will be written entirely in Welkin.*
- The initial implementation, pywelkin, will only prioritize on the core library and cli. *This project will no longer make GUI applications.* In the near future, there will be support for existing text editors and programs (TBA). This means the project can leverage current editors *instead* of developing one first. I am making GUI applications in the future, but those will be (you guessed it) *specified in Welkin.*
    - Some of the tooling may change as well. I did switch from poetry to pdm (due to Linux based issues), but I may switch back. In any case, *dependencies should be as minimal and portable as possible.* More features will be supported through plugins in a separate repository (TBA).

**In short,** this repository will now focus on the Welkin language. Formal tools, utilities, and more will be the focus of new projects (coming soon!).

**Logo and Timelapse: TBD**

Welcome to Welkin, an all-purpose knowledge manager (AIM)! You can write about *any* and *all* pieces of information you wish to keep. It's a special programming language *specially designed for information!*

-   Writing a screenplay? Store all of your key events and characters into their dedicated nodes, interweaving them as you develop the plot.
-   Have a bunch of scrambled notes from a class? Put your key ideas into nodes and interconnect them, allowing you to easily traverse what you jotted down, and make it easy to keep adding on.
-   Working on a programming project? Store each key function in its own node, full with documentation and overall structure. Keep your implementation inside the node and better understand how every component works.

But this list is not exhaustive; the sky is the limit!

# What does "Information" Mean?

I'm using it as a general term, broadly meaning "anything related to your perception or thought". My definition comes from the [<https://etymonline.com/word/information>](etymology of information] (with added emphasis):

> from Latin informationem (nominative informatio) "outline, concept, idea" noun of action from past participle stem of informare "to train, instruct, educate; **shape, give form to**";

The way you perceive or think about the world creates unique *forms*, which is what I am calling information.

Note that information doesn't need to be true. It could be ficitious (in a book or screenplay). It definitely doesn't need to be *knowledge*, but I would claim its underlying structure *does* provide knowledge. Now, that is a rabbit hole in of itself, and I will not get to that here. (There will be an extension that handles verification and knowledge exactly: TBA). 

Needless to say, it's nice to have a broad definition. Most importantly, you can, and should, write **everything** down! In my opinion, *every piece of information formed is valuable in of itself.* 

- Have a mistake? You'll want to keep it for later! It could help someone else down the road
- Think you're getting stuck on a problem? Who knows what you have written; maybe it could apply in the future or even apply *to something else entirely*
- And the list goes on

But, I hear you asking, how do I manage all of these notes? That's where some of the core features of Welkin come in: not only can you store *everything*, you can easily navigate it!


# But What IS Welkin?

That answer depends on how you perceive Welkin. From the outset, Welkin is a tool to handle labeled (finite) [graphs](https://en.wikipedia.org/wiki/Graph_(discrete_mathematics)) (or networks). That's it! It can determine whether two graphs have the same structure, *no matter how you name it!* Everthing you do is fundamentally based on combinations and connections, no matter how many you have! Plus, you can do some special things with the computer, with a special (optional) component for making *any* program! Note that you can write Welkin, the language, pretty much *anywhere,* including good ol' paper and pencil. (I will have protocol templates you can use to help you transfer between paper and digital notes: TBA).

However, philosophically, Welkin is based on a theory called Continuum Foci Logic and Theory (CFLT). This theory is heavily inspired by both Western and Eastern thought and aims to provide a unified theory of epistemology and ontology. It is currently in the works, with some of my ideas posted on my blog: [Wild Perpetual Curiosities (WPC)](https://wildperpetualcuriosities.wordpress.com). Over time, CFLT will be described in Welkin! That way, you can pretty much describe *anything.* You can use Welkin without knowing anything about this; the role of CFLT is to *emphasize* and *enhance* the inherent capaibilites of Welkin. (As I will eventually prove, Welkin is extremely powerful!)

Welkin, as a program, does need to be standardized for *everyone* to use. (Otherwise, it would be a bit chaotic).* To satisfy this need, there is an [official book (WIP)](https://github.com/Astral-Bear-Studios/welkin-book) fully describing how Welkin, the program, works, as well as a formal specification for the Welkin language. Welkin stores information in meta-graphs, which means *anything* can be a node, including edges or other graphs! *This has yet to be seen, but Welkin aims to be a universal format. Imagine comparing structures from completely different disciplines! In this sense, Welkin is a universal (written) language!*


# (Planned) Features

-   Zoom in/out of ideas
-   Always have the option to extend on information
-   Customize the way you perceive them
-   Always have a mechanism to defeat repetitive structures
-   Long Term: Accessibility and Human Language Support


# Development: TBA

For cross-platform usage and ease of usage, the first official implementation of this project is in python, called [PyWelkin](https://github.com/astral-bear/pywelkin).

There will be dedicated files for the roadmaps, updates, etc. Eventually, these will be written in .welkin files, serving as a unified way to communicate ideas for the project (and *all* related projects).

**Lead Developer:** Oscar Bender-Stone

**Please email oscarbenderstone@gmail.com if you would like to be a contributor. I have yet to make the guidelines, but I am open to any recommendations as I am writing them.**

