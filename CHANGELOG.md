# Change Log (Temporary)

**Status: In use**

All changes and updates for Welkin will be stored here.
This document will eventually be superseded by a new file, which will compile into Welkin. 

## 2024-21-3

Two major structural changes.

### Added

- Updates will be put into a changelog for easier access. Please see CHANGELOG.md for future reference. Dates will be written in ISO notation yyyy-mm-dd to minimize confusion. If a new format is chosen in the future, it will be put into this document first.

### Removed
- Due to their complexity, there will no longer be git submodules for welkin-book and pywelkin. Instead, this README will only include links. Interested contributors can clone which projects they would like to work on.
This will be the last update put in this README.

## 2024-27-24

Major update to entire project.

I have realized that the Standard and initial implementation aimed to do too much and had scope creep. I realized that Welkin does not need to do everything in one go and emphasize how it is a *universal information format.* This means two big things for the project.

## Changed
- The Standard will prioritize on one task: *formally specify* the Welkin language:
    - Syntax: Has a precise LALR grammar, with details on every terminal and rules.   
    - Semantics: Defines a WIG (Welkin Information Graph) and its notion of equivalence.
Every possible detail will be considered, in order to avoid ambiguities in other formats (including JSON). In order to simplify things and avoid confusion, there will no longer be any variants: there will be *exactly one grammar* and semantics for reference. Because Welkin is self-contained, *the Welkin interpreter will not be specified.* Instead, *the interpreter's specification will be written entirely in Welkin.*
- The initial implementation, pywelkin, will only prioritize on the core library and cli. *This project will no longer make GUI applications.* In the near future, there will be support for existing text editors and programs (TBA). This means the project can leverage current editors *instead* of developing one first. I am making GUI applications in the future, but those will be (you guessed it) *specified in Welkin.*
    - Some of the tooling may change as well. I did switch from poetry to pdm (due to Linux based issues), but I may switch back. In any case, *dependencies should be as minimal and portable as possible.* More features will be supported through plugins in a separate repository (TBA).

**Overall:** this repository will now focus on the Welkin language. Formal tools, utilities, and more will be the focus of new projects (coming soon!).
