### Propsals under construction
This directory contains `generate_html.sh` and one markdown file per proposal:
* `P3832.md` for [`P3832`](https://wg21.link/p3832) - Timed lock algorithms for multiple lockables
* `P3833.md` for [`P3833`](https://wg21.link/p3833) - `std::multi_lock`

To generate the html version of the document you're interested in:

Example:
```
$ ./generate_html.sh P3833.md
P3833R2a.html
```
`R3b` here means the second (`b`) pre-release of `R3`. When submitting the propsal, it'll first be named `R3` and committed. Directly after committing and submitting the proposal, a new version, `R4a` should be committed.

#### Editing a proposal
Just edit the markdown file and keep track of numbering. `generate_html.sh` doesn't do renumering.
Be aware of that `generate_html.sh` only knows a few keywords that it uses for converting specification clauses into lists with three columns. These are currently:
Constraints, Preconditions, Effects, Postconditions, Returns, Throws, Error conditions
