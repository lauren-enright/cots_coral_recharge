*merged dataframe that is made in script 1, and read in for script 2* 
*cots_haplo_timeline_10062025.csv*

Enrichment_trt:	This is the enrichment treatment. Plots are either Enriched or Ambient. Plots that are Enriched have nutrients added with fertilizer-filled nutrient diffusers. Note that the enrichment treatments ended in T12 (Summer 2022) and all plots have had ambient nutrients since then 
Block_Plot_Trt:	Location of the coral. Block plot (A3, A4, B1, B2, C2, C4, D1, D3) and treatment (1x1, 2x2, 3x3, open). 
Un_ID:	Unique ID for each coral
Herbivory_trt:	This is the consumer pressure treatment. Treatments are 1X1, 2x2, 3X3, and open, which correspond to very low, low, medium, and high levels of herbivory and corallivory
Coral_ID:	The correct coral ID's for all corals. Use these. These are the ID's used for the "Un_ID" column.
Plot:	The plot in which the coral is located. Plots are A3, A4, B1, B2, C2, C4, D1, D3. Each plot has 4 exclosures, each with a different level of herbivory
Haplotype:	the mtORF haplotype from Sanger sequences
Species:	The species name
flag_uncertain_recruit_time: 1 = Recruitment_timepoint was uncertain. 0 = Recruitment_timepoint is known, can use
flag_partial_mortality: 1 = Partial mortality. 0 = No partial mortality
flag_unlabelled: 1 = "Poc in bags" samples sampled from the new tiny recruits in plots C and D, but which the datasheets were temporarily misplaced which allow us to figure out which samples are which.
flag_bad_sequence: 1 = sample was sequenced but the mtORF sequence was poor quality, so no Species given; 0 = mtORF sequence was good and a Species name is provided
flag_missing_sample: 1 = no tube or sample was provided; 0 = sample was provided
Coral_Genus: Coral genus (Poc or Acr). The COTS order of consumption data was taken for Poc and Acr. 
Timepoint: Timepoint of Demographic Data 
Recruited: Whether this coral was recruited in a particular timepoint
Alive: 1 if coral is alive, 0 if either Dead_COTS, PartialDead_COTS, Dead_Other, or PartialDead_Other
Dead_COTS: 1 if coral is dead by COTS, 0 if either Alive, PartialDead_COTS, Dead_Other, or PartialDead_Other
PartialDead_COTS: 1 if coral is partially dead by COTS, 0 if either Alive, Dead_COTS, Dead_Other, or PartialDead_Other
PercPartialDead_COTS: percent partially dead by COTS, NA if not partially dead by COTS
Dead_Other: 1 if coral is dead from a cause that is not COTS, 0 if either Alive, Dead_COTS, PartialDead_COTS, or PartialDead_Other
PartialDead_Other: 1 if coral is partially dead from a cause that is not COTS, 0 if either Alive, Dead_COTS, PartialDead_COTS, or Dead_Other
PercPartialDead_Other: percent partially dead by not COTS, NA if not partially dead 
Important_Notes: important notes about coral. these are a subset of all notes taken in the field.
COTS_T15: The exclosures were designed to keep fish out, not COTS. Some plots were more susceptible to COTS invasions than others. A 1 means that a COTS was able to get into the plot and a 0 means that we do not believe COTS were able to access that particular cage at T15
COTS_T16	The exclosures were designed to keep fish out, not COTS. Some plots were more susceptible to COTS invasions than others. A 1 means that a COTS was able to get into the plot and a 0 means that we do not believe COTS were able to access that particular cage at T16

Raw Data Read into Script 1:

*Timeline for when COTS got into particular cages*
recharge_COTS_timeline.csv

Block_Plot_Trt	Location of the coral. Block plot (A3, A4, B1, B2, C2, C4, D1, D3) and treatment (1x1, 2x2, 3x3, open). 
Enrichment_trt	This is the enrichment treatment. Plots are either Enriched or Ambient. Plots that are Enriched have nutrients added with fertilizer-filled nutrient diffusers. Note that the enrichment treatments ended in T12 (Summer 2022) and all plots have had ambient nutrients since then 
COTS_T15	The exclosures were designed to keep fish out, not COTS. Some plots were more susceptible to COTS invasions than others. A 1 means that a COTS was able to get into the plot and a 0 means that we do not believe COTS were able to access that particular cage at T15
COTS_T16	The exclosures were designed to keep fish out, not COTS. Some plots were more susceptible to COTS invasions than others. A 1 means that a COTS was able to get into the plot and a 0 means that we do not believe COTS were able to access that particular cage at T16

*Data for if/when COTS ate particular RECHARGE corals*
COTS_RECHARGE_Poc_10032025.csv
Un_ID:	Unique ID for each coral
Coral_ID:	The correct coral ID's for all corals. Use these. These are the ID's used for the "Un_ID" column.
Block_Plot_Trt:	Location of the coral. Block plot (A3, A4, B1, B2, C2, C4, D1, D3) and treatment (1x1, 2x2, 3x3, open). 
Plot:	The plot in which the coral is located. Plots are A3, A4, B1, B2, C2, C4, D1, D3. Each plot has 4 exclosures, each with a different level of herbivory
Herbivory_trt:	This is the consumer pressure treatment. Treatments are 1X1, 2x2, 3X3, and open, which correspond to very low, low, medium, and high levels of herbivory and corallivory
Coral_Genus: Coral genus (Poc or Acr). The COTS order of consumption data was taken for Poc and Acr. 
Timepoint: Timepoint of Demographic Data 
Recruited: Whether this coral was recruited in a particular timepoint
Alive: 1 if coral is alive, 0 if either Dead_COTS, PartialDead_COTS, Dead_Other, or PartialDead_Other
Dead_COTS: 1 if coral is dead by COTS, 0 if either Alive, PartialDead_COTS, Dead_Other, or PartialDead_Other
PartialDead_COTS: 1 if coral is partially dead by COTS, 0 if either Alive, Dead_COTS, Dead_Other, or PartialDead_Other
PercPartialDead_COTS: percent partially dead by COTS, NA if not partially dead by COTS
Dead_Other: 1 if coral is dead from a cause that is not COTS, 0 if either Alive, Dead_COTS, PartialDead_COTS, or PartialDead_Other
PartialDead_Other: 1 if coral is partially dead from a cause that is not COTS, 0 if either Alive, Dead_COTS, PartialDead_COTS, or Dead_Other
PercPartialDead_Other: percent partially dead by not COTS, NA if not partially dead 
Important_Notes: important notes about coral. these are a subset of all notes taken in the field.

*From previously published paper*
Species IDs.csv 
Un_ID: Unique ID for each coral
Plot: The plot in which the coral is located. Plots are A3, A4, B1, B2, C2, C4, D1, D3. Each plot has 4 exclosures, each with a different level of herbivory
Herbivory_trt: This is the consumer pressure treatment. Treatments are 1X1, 2x2, 3X3, and open, which correspond to very low, low, medium, and high levels of herbivory and corallivory
Enrichment_trt: This is the enrichment treatment. Plots are either Enriched or Ambient. Plots that are Enriched have nutrients added with fertilizer-filled nutrient diffusers.
Coral_Id: The correct coral ID's for all corals. Use these. These are the ID's used for the "Un_ID" column. These reflect all corrections. For most corals "Coral_ID" and "Coral_ID_past" are exactly the same. They only differ if we made corrections in the "Coral_ID_field" or "Coral_ID_corrected" columns.
Haplotype: the mtORF haplotype from Sanger sequences
Species: The species name
flag_uncertain_recruit_time: 1 = Recruitment_timepoint was uncertain. 0 = Recruitment_timepoint is known, can use
flag_partial_mortality: 1 = Partial mortality. 0 = No partial mortality
flag_unlabelled: 1 = "Poc in bags" samples sampled from the new tiny recruits in plots C and D, but which the datasheets were temporarily misplaced which allow us to figure out which samples are which.
flag_bad_sequence: 1 = sample was sequenced but the mtORF sequence was poor quality, so no Species given; 0 = mtORF sequence was good and a Species name is provided
flag_missing_sample: 1 = no tube or sample was provided; 0 = sample was provided
