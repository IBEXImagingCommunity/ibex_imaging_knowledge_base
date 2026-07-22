---
layout: default
---


# Reagent Contribution Shortcut Instructions

Welcome to the reagent contribution shortcut, where we work together to enable you to easily add reagent information to the Knowledge-Base. You provide the scientific information, and we take care of the technical parts (git, GitHub, formatting).

Please read the general [contribution instructions](../contrib.md) before proceeding. Primarily, familiarize yourself with the expected supporting image conventions if you intend to provide supporting images.

You will need to provide us with the following:
1. A csv with the columns listed in [this example](new_entries.csv). This csv is similar to the one used by the Knowledge-Base and contains two additional columns, `Publications`,and `Notes`.
2. `Publications` column - If there are one or more publications associated with a reagent validation, list each one in a markdown file [like this one](pub1.md) and reference them in this column (file names are separated by a semicolon). If there are no publications, leave the column entry empty.
3. `Notes` column - If there are notes that you would like to provide, information that is not listed in any of the columns, this is where to provide it. For example "This alpha smooth muscle actin antibody labels cytoskeleton proteins in various mouse tissues. In the tumor, the AF488 conjugate (53-9760-82) works very well and labels actin family of proteins, smooth muscle cells, and cancer associated fibroblasts." If there are no notes, leave the column entry empty.
4. `Image Files` column - If you have one or more images that support the specific validation, list them in this column (file names are separated by a semicolon). Note that the same file may support multiple validations and we only keep a single copy of it. Consequentially, you will need to decide in which directory (`target_conjugate` directory name) you want the image to reside. In the [example](new_entries.csv) we have two image files and both will reside under a directory `BCL2_Unconjugated`.

Finally, provide the image files in a single directory. Use meaningful image file names similar to those provided in the [example directory](images).
