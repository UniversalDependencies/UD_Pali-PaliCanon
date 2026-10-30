# Summary

UD_Pali-PaliCanon is the first UD treebank for the Pāli language containing manual annotations of sentences from [the Pāli Canon](https://en.wikipedia.org/wiki/Pali_Canon).  We have only just begun to annotate the Pāli Canon and we welcome help to expand our coverage!

# Description

The Pāli Canon is the sacred literature of Theravāda Buddhism.
We take as our source the Public Domain, Mahāsaṅgīti edition [widely available online](https://tipitaka2500.github.io/), though other editions are also Public Domain and are broadly similar.

Following [the UD guidelines for Pāli annotation](https://universaldependencies.org/pi), we strip out all punctuation and normalize the text to the IAST format, i.e. we represent the *niggahīta* with an m-underdot ("ṃ").
Because the extant editions inconsistently use punctuation, we do not naively trust their punctuation for sentence tokenization but rather split our text into sentences by hand based on syntax.
We prefer small, syntactically valid sentences over run-ons wherever possible.
Instead of punctuation, UD Pāli uses a capital letter to represent the start of a new sentence.

For sentence ids, we use SuttaCentral's [segment ids](https://suttacentral.net/numbering?lang=en).
When we split one SuttaCentral segment into multiple sentences, we append `_1`, `_2`, etc to the end of the segment id to mark its order within the segment.

This treebank is still a work-in-progress and is being actively updated and expanded on a regular basis.
We currently have only 2049 of the approximately three million words of the Pāli Canon annotated, in 222 sentences from the Mahāpadānasutta (DN 14).

# AI Policy

All contributions to this treebank must be manual annotations as defined by the UD documentation.

In our research (Lin, Singh, and Khemarato 2026), even frontier LLMs require significant [hand-holding](https://docs.google.com/document/d/1JuMfqXiSny8o1J4PbzxIazYGqJGlj1x0c4nUf90gqgA/edit?usp=sharing) and careful, manual review to produce accurate CoNLL-U for Pāli.

# Acknowledgments

...

## References

* Lin, Chia-Wei, Jasvinder Singh, and Khemarato Bhikkhu. 2026. "PāliUD: Prompt-engineered annotation and philological evaluation for the Pāli Treebank." In Proceedings of the 22nd Conference on Natural Language Processing (KONVENS 2026). Hamburg: University of Hamburg.

# Changelog

* 2026-11-15 v2.19
  * Initial release in Universal Dependencies.


<pre>
=== Machine-readable metadata (DO NOT REMOVE!) ================================
Data available since: UD v2.19
License: CC BY-SA 4.0
Includes text: yes
Parallel: no
Genre: nonfiction
Lemmas: manual native
UPOS: manual native
XPOS: not available
Features: manual native
Relations: manual native
Contributors: Lin, Chia-Wei; Singh, Jasvinder; Bhikkhu, Khemarato
Contributing: here
Contact: khemarato.bhikkhu@gmail.com
===============================================================================
</pre>
