################################################################################
# tagset.dat
################################################################################
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


################################################################################
# locucions.dat and locucions-COMPLETE.dat
################################################################################
FreeLing's handling of multi-word phrases (MWPs), which involves lemmatizing the
2+ word phrases as a single lemma, is not a good strategy. It requires corpus
users to either (a) know all 2100 or so multi-word phrases when performing queries
and search for them as a single compounded word, or (b) accept that their queries
of components of MWPs will not return the MWPs (e.g. a search for "a" will not
return instances of "a través de" because this is lemmatized as "a_través_de".

Therefore, the locucions.dat file has been trimmed down to the bare minimum. The
original Chilean Spanish MWP file is still available as "locucions-COMPLETE.dat".


################################################################################
# probabilitats.dat
################################################################################
This file contains just a few modifications of the previous version - "hm" and
"mm" as interjections now have higher probabilities of being an interjection
rather than "hectómetro" and "milímetro".
