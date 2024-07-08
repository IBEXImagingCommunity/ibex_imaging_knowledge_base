---
layout: default
---

# Questions and Answers

This file contains questions and answers addressing various aspects of the knowledge-base, IBEX and related methods, and software details that were not addressed in publications or which were not sufficiently clear to scientists from their descriptions in the publications.

---

If you have a question that does not appear here, please ask on the [knowledge-base GitHub Discussions](https://github.com/IBEXImagingCommunity/ibex_imaging_knowledge_base/discussions). Posting to the Discussions board requires a GitHub account. If you do not have an account, please follow these [instructions to sign up for one](https://docs.github.com/en/get-started/signing-up-for-github/signing-up-for-a-new-github-account).

---

## Knowledge-Base

1. **How do I contribute to the IBEX knowledge-base?**  
Thank you for joining us! Please see instructions on how to contribute [here](contrib.md). 

1. **Do you support other multiplexed imaging methods other than IBEX?**  
Yes, the IBEX knowledge-base includes antibodies validated for Multiplexed 2D Imaging, Ce3D, Ce3D-IBEX, Opal-plex, and Cell DIVE-IBEX. Please see the [glossary](./contrib.md#glossary) for additional details. The knowledge-base does not presently support antibodies validated for other highly multiplexed imaging methods using antibody removal or other dye inactivation protocols.

1. **How do I find the RRID for an antibody?**  
Many antibody companies list RRIDs on their product pages (BioLegend, BD Biosciences, Miltenyi Biotec, Thermo Fisher Scientific). If an RRID is not listed, then please search the [RRID Portal](https://scicrunch.org/resources). If an antibody does not have an RRID, then please consider [registering it](https://antibodyregistry.org/add).

1. **How do I find the UniProt ID for an antibody target?**  
Please see [uniport.org](https://www.uniprot.org) for completing primary antibody entries. For secondary antibodies and other reagents, please insert “NA” in the UniProt Accession Number column of the reagent_resources.csv file.

## IBEX Method

1. **Is IBEX compatible with FFPE samples?**  
Yes! The use of IBEX on heavily fixed mouse FFPE samples using Opal-plex is shown in [[Figure 6, Radtke et al. 2020](https://doi.org/10.1073/pnas.2018488117)] and in [[Figure 4, Radtke et al. 2022](https://doi.org/10.1038/s41596-021-00644-9)] for human FFPE samples using automated IBEX. Additionally, the manual IBEX method, [[Figure S3A, Radtke et al. 2020](https://www.pnas.org/doi/suppl/10.1073/pnas.2018488117/suppl_file/pnas.2018488117.sapp.pdf)], can be applied to FFPE tissue sections adhered to glass slides. For a complete list of antibodies evaluated for FFPE samples see the reagent_resources.csv file.

1. **Is LiBH4 safe to use?**  
IBEX has been performed hundreds of times by dozens of junior and senior investigators in the laboratory. Please follow the safety instructions describe in the [protocols](https://doi.org/10.1038/s41596-021-00644-9):  
*“Perform these steps in a chemical hood with appropriate PPE. Always work with small amounts (<10 mg) of LiBH4. Replace vial of LiBH4 after 4 weeks of prolonged use as we have observed reduced bleaching efficiency after repeated exposure to air. We recommend purchasing the smallest aliquot (1 g) available. Alternative borohydride solutions may also be considered and empirically tested for their compatibility with the fluorophores and panels described here.”*   
**Please make sure to train all members of your lab in the safe handling of all reagents used for IBEX.**

1. **What imaging substrates are compatible with IBEX?**  
The IBEX2D Manual method was originally described using a two-well chambered coverglass and an inverted microscope. This configuration allowed samples to be iteratively imaged without adding and removing a coverslip after each cycle, preventing tissue loss while simplifying execution of the protocol. The IBEX2D Manual method has also been demonstrated using a glass slide and upright and inverted microscopes [[Figure S3A, Radtke et al. 2020](https://doi.org/10.1073/pnas.2018488117)]. The IBEX2D Automated method employs tissues sectioned onto glass coverslips and imaged using an inverted microscope [[Radtke et al. 2022](https://doi.org/10.1038/s41596-021-00644-9)].

1. **How does one prepare sections for the two-well chambered coverglass?**  
Please see Steps 1-4 in Box 2 [[Radtke et al. 2022](https://doi.org/10.1038/s41596-021-00644-9)] for detailed instructions on how to prepare tissue sections using a cryostat. For best results place a two-well chambered coverglass into the cryostat 10 minutes before sectioning. This prevents the tissue sections from adhering to the warm surface before they are optimally placed. Cut several test sections onto glass slides. These test sections are useful for control staining and panel design. Use paintbrushes to carefully flatten the tissue section. Once flattened, pick up the tissue section with delicate, flat-edged forceps (MilliporeSigma Filter Forceps, Catalog number XX620000P). Place the section into the middle of the coated well as shown in the [Extended Data Figure 1](https://doi.org/10.1038/s41596-021-00644-9#Fig1). Use a paintbrush to flatten onto glass. Place your finger underneath the section to gently melt the tissue onto the bottom of the glass well. Dry sections onto coated two-well chambered coverglass for one hour at 37 degrees Celsius or overnight at room temperature.

1. **What materials are required to set up IBEX in the laboratory?**  
Please see [[Radtke et al. 2022](https://doi.org/10.1038/s41596-021-00644-9)] for an extensive material and equipment list. [Table S4](https://doi.org/10.1038/s41596-021-00644-9#MOESM1) additionally includes estimated costs for IBEX implementation.

1. **What is a fiducial and how do you select one for your experiments?**  
A fiducial is a marker that is present in all imaging rounds and used for image registration. IBEX is compatible with a wide range of fiducials as demonstrated in the original publication: nuclei, vessels, and immune cells [[Figure 3, Radtke et al. 2020](https://doi.org/10.1073/pnas.2018488117)]. It is recommended to select an antibody or nuclear dye that labels cells and structures throughout a tissue section and maintains a robust signal after prolonged exposure to LiBH4.

1. **Are antibodies removed from the tissue after LiBH4 treatment?**  
No, LiBH4 extinguishes the fluorescence signal but does not strip antibodies from the tissues [[Figure S2, Radtke et al. 2020](https://www.pnas.org/doi/suppl/10.1073/pnas.2018488117/suppl_file/pnas.2018488117.sapp.pdf)].

1. **Are Chrome Alum-Gelatin coated slides and/or imaging chambers required for IBEX?**  
Yes, using substrates coated with this adhesive is highly recommended. Chrome Alum-Gelatin is required to maintain tissue integrity over dozens of imaging rounds. Charged glass slides are not sufficient and will result in tissue lifting and loss. If you are unable to obtain Chrome Alum-Gelatin through a supplier, then you can prepare this reagent from several recipes [available online](https://www.laboratorynotes.com/preparation-of-chrome-alum-containing-gelatin-solution-for-preparation-of-coated-slides-for-histological-tissue-sections/).

1. **What mounting media are compatible with IBEX?**  
It is imperative to use a water soluble mounting medium that can be removed to allow iterative rounds of imaging. Using Fluoromount-G is highly recommended. 

1. **Is a scientific microwave required for immunolabeling?**  
No, thin tissue sections (<10 microns) can be immunolabeled in 1 hour at 37 degrees Celsius.

1. **What is the best way to remove the coverslip for the IBEX2D Manual method without destroying the tissue?**  
First, use a non-curing, water soluble mounting medium (Fluoromount-G). Place the slide with coverslip into a 50 ml falcon tube filled with PBS. After 10 minutes, dip the slide several times in and out of the PBS. The coverslip should float off on its own. If it does not, then wait an additional 5 minutes and repeat. It may be necessary to use a forceps to gently lift one corner of the coverslip to allow the PBS to make contact with the tissue.

## Software

1. **When following the SimpleITK Imaris Extensions [setup instructions](https://github.com/niaid/imaris_extensions#setup) I get the following error, "CondaHTTPError: HTTP 000 CONNECTION FAILED for url...". What should I do?**  
This error is most likely due to your institution's proxy server security settings. To resolve proxy server issues, see the [instructions provided in the anaconda documentation](https://docs.anaconda.com/working-with-conda/reference/security/#using-anaconda-behind-a-company-proxy) and possibly the instructions for using [non standard certificates](https://conda.io/projects/conda/en/latest/user-guide/configuration/non-standard-certs.html).
This [stack-overflow discussion](https://stackoverflow.com/questions/33883371/python-anaconda-proxy-setup-via-condarc-file-on-windows) may also be of interest.  
Another possible solution is to install packages from PyPi using the `requirements.txt` file found in the source root directory:  
    ```
     conda create -n imaris python=3.7.0
     conda activate imaris
     pip install --upgrade pip
     pip install -r requirements.txt
    ```

1. **I am using the registration application from the [imaris extensions GitHub repository](https://github.com/niaid/imaris_extensions) and it fails. Are there settings I can change to make it work?**  
Yes. For common failure modes and various settings that you can try, see the application's `Help` menu or [this web page](https://niaid.github.io/imaris_extensions/XTRegisterSameChannel.html).
