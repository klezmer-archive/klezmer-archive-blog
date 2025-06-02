---
title: "Encoding in MEI: \"Hannah's Skotshne\""
date: 2025-06-02T16:39:54.646Z
authors:
  - Clara Byom
description: "Encoding annotations, different readings, and more! (You don't
  need to code to understand this blog post!) "
tags:
  - MEI
categories:
  - Klezmer
---
### Manuscript to Encoding

\
Ah, our beloved "Hannah's Skotshne" (KMDMP 20-59-1676).

By now, many of you have heard the tale of this tune that has swept around the globe since the launch of the Kiselgof-Makonovetsky Digital Manuscript Project (KMDMP). The original manuscript captured in the photo is torn, folded, and worn to the point of illegibility. 

**Image 1: Facsimile of the "Hannah's Skotshne" Manuscript**

![Image 1: Facsimile of the "Hannah's Skotshne" Manuscript](/images/uploads/kmdmp-20-59-1676-edited.png "Image 1: Facsimile of the \"Hannah's Skotshne\" Manuscript")

Nevertheless, KMDMP digitizer extraordinaire Hannah Ochner tackled this piece, providing us with a legible version of the tune from the bits of writing peeking out from the folds and context throughout the tune. When Hannah was done, she submitted her MusicXML file for us to reference as we move into the editorial phase of encoding using MEI. 

MEI is a XML specification (a version of the musicXML produced by music notation programs) developed by the Music Encoding Initiative used widely for digitally encoding music in academic and archival projects with similar goals to the Klezmer Archive. The schema is developed in the open and the project leaders welcome changes from the community. Indeed, we have already contributed a few small changes that have been accepted and will be included in future releases. The community also has built a suite of tools that we are excited to use, including the Verovio renderer and MEI-friend editor.



### Why MEI?

MEI allows us to document more details than a typical notation software, including representing ambiguous marks in handwritten scores and supporting editorial annotations. Within a ***single document*** we can capture the "manuscript" version (replicates what we see on the page as closely as possible) and an "edited" version (klezmorim-informed, playable version that makes corrections or clarifies ambiguities on the manuscript). This means that rather than printing multiple versions and comparing them measure by measure, we can highlight these differences and the user can choose what version to display depending on their use for the document at the moment! The ability to encode multiple readings of the manuscript (e.g. original, amended/edited, and playable) in a single document allows the MEI file to be the "single source of truth" for the digital notation. MEI encoding not only allows users to render the different readings of the tune for print or screen, it also makes the annotations and editorial notes available to the graph database that contains the complete record for this item.

In May of 2024, I set out to learn MEI and (foolishly?!?) decided to begin with "Hannah's Skotshne." Over the course of the following year, Max Rothman and I had numerous meetings to understand how best to reflect the whole of the tune in a single encoded document. The complexity of "Hannah's Skotshne" was perfect for exploring the differences between our desired versions, determining what level of detail was necessary vs. too much, and sorting out how to tweak MEI to fit our unique needs. We're still working on our specific editorial policy (which is informed by our KMDMP Scholarly Editions Policy too!) and many details are unnecessary to relay in full here, but we do want to highlight some of the fun challenges we've encountered so far.



### C﻿hallenge #1: The Key Signature

Most notation softwares allow us to create our own key signatures, including the one found on the manuscript with B-flat, E-flat, and C-sharp. What is tricky to document in this instance is the presence of two "hands" that created this key signature and the implications for every instance of the C-sharp throughout the remainder of the code. 

The individual who wrote this tune down in the alter klezmer-heft (old klezmer notebook) has written it fully with just a B-flat and E-flat in the key signature, marking the C's throughout the tune with an accidental. The purple C-sharp matches the writing implement that marks the K-numbers throughout the manuscript, likely Moishe Beregovski, to whom the catalog in Yiddish is attributed.

**Image 2: Modal key signature on the "Hannah's Skotshne" manuscript**