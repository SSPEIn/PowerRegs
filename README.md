# PowerRegs
This repo aims to maintain a version-controlled repository of Indian grid regulations in plaintext format. 

## Background
Regulations used to be originally printed in the respective (Central or State) Gazette book. They became PDF scans of the relevant pages of the Gazette, which sometimes then became soft copies of those pages. More usefully, many times the Gazette notification started to be released in machine-readable PDF form.

A major issue arises with amendments, which are basically procedural substitutions written in human language.

The problem, then, is that at any point in time, there is not necessarily available an up-to-date version of the regulations unless the ERC explicitly releases one (which have been rare in practice).

Further, there is an unnecessary amount of human labour involved in understanding what the true effect of each amendment is.

Ultimately all these problems can be solved by making the procedural substitutions machine-readable. This repo aims to do just that by using modern version control (Git has been chosen as of now) to represent the amendments.

## Structure
Each folder represents a body, typically an ERC but might also include ministries that issue rules and amendments to such rules.

Each plaintext file represents one regulation. The format is `<short name>_<year>.txt`

## Version control
Each commit represents one amendment, with the (commit/author) date being the date on which it went into effect as per the Notification.

This way of doing things has one important limitation, but it is largely a burden on the author (i.e. me at this point) - since commits represent amendments, any changes I make (corrections, clarifications, etc) to the content of the regulations involve a complete rewrite of the repository. 

The downside to users is that commit hashes cannot be guaranteed to be stable. This limitation cannot be really lifted without a much more sophisticated solution which does not yet have adequate tooling to be usable. Even so, I believe and hope this repo will be valuable to Indian power sector professionals.


