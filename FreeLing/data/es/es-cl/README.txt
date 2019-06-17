The tagset.dat file in this directory contains a modified tagset that is used
with the Sociolinguistic Corpus of Chilean Spanish (COSCACH). The modifications
include the following:

- The last position in pronoun and verb POS tags ("polite" and "gender",
  respectively) has had the value "voseo" added.
- The 5th column tags are now a 1-capital-letter POS tag.
- The 6th column tags are now 3-lower-case-letter POS sub-tags.

If you use the CL.tanc.Vos-V, CL.vaux.Vos-V and CL.verb.Vos-V dictionary files
(in which voseo verb POS tags and the "vos" pronount tag have a final "V"), then
you have two options:

    - Use this modified tagset.dat file, which will avoid error messages when
        tagging voseo verbs or the pronoun "vos" with FreeLing.
    - Use the general Spanish tagset.dat file, which will cause errors to be
        thrown when tagging voseo verbs or the pronoun "vos" with FreeLing,
        but will not otherwise affect tagging.

If you use the default Spanish dictionary files CL.tanc, CL.vaux and CL.verb, you
*can* use this modified tagset.dat file, and you will get the modified 5th- and
6th-column tags, but voseo-related words will receive the same tags as tuteo-related
words (this is FreeLing's default behavior).
