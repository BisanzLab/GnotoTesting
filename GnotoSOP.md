# GNO 004 Isolator Microbial Testing

## 1. Scope

This SOP applies to any personnel involved in the testing of the isolators.

## 2. Purpose

The purpose of this procedure is to maintain consistency in the testing of isolators to avoid contaminating the results and to maintain sterility. Sterility is tested both through aerobic and anaerobic culture, as well as quantitative PCR as a culture independent method.

## 3. Definitions

|Term|Definition|
|-|-|
|SOP|Standard Operating Procedure|
|MSDS|Material Safety Data Sheet|
|ARP|Animal Resource Program|
|MST|Microbial Swab Test|
|TSB|Tryptic Soy Agar with 5% Sheeps Blood|
|BHI CHVR| Brain Heart Infusion with Cysteine, Hemin, Vitamin K, and Rezasurin|
|Ct|Threshold Cycle of Detection|

## 5. Procedure

### Materials and Equipment Needed

|Item|Storage|Ordering Information|
|-|-|-|
|Microbial Swab Test|RT| |
|TSB agar|4˚C| See [recipe](https://github.com/BisanzLab/LabProtocols/blob/main/BacterialMedia.md)|
|BHI CHVR agar and broth|4˚C| See [recipe](https://github.com/BisanzLab/LabProtocols/blob/main/BacterialMedia.md)|
|Oligos|-20˚C|See Table 5.1|
|ZymoBIOMICS 96 MagBead DNA Kit|RT|Zymo D4302 OR D4308|
|Bio-Rad 96 Well Plate 200 µL skirted PCR plate|RT|Biorad HSP9601|
|384 Plates for qPCR|RT|Biorad #HSP3865)|
|Optically clear Plate Seals (Microseal ‘B’) |-|Biorad  #MSB1001|
|iTaq Universal Probes Supermix|-20˚C|BioRad 1725132|
|2 x Opentrons filter 200ul tips|RT|[link](https://shop.opentrons.com/collections/opentrons-tips/products/opentrons-200ul-filter-tips)|
|2 x Opentrons filter 20ul tips|RT|[link](https://shop.opentrons.com/collections/opentrons-tips/products/opentrons-20ul-filter-tips)|
|CFX384 Thermocycler|-|-|
|Biospec Mini-Beadbeater-96 or similar|-|-|
|Opentrons OT-2 with gen 2 Magnetic module, 20ul single channel, 300ul multichannel, and tube rack.|-|-|
|Anaerobic Chamber with >0% CO2 or Anaerobic Jar|-|-|
|37˚C Degree Incubator|-|-|
|PCR Laminar Flow Hood|-|-|

**Table 5.1: Oligos in 10X Assay Mix**
|Oligo|Sequence|Stock [µM]|Working [µM]|Final [nM]|
|-|-|-|-|-|
|891F|TGGAGCATGTGGTTTAATTCGA|100|2|200|
|1003R|TGCGGGACTTAACCCAACA|100|2|200|
|1002P|	 [6FAM]CACGAGCTGACGACARCCATGCA[BHQ1]|100|2|200|


### Sampling Frequency

All isolators housing mice will be tested on a monthly basis, either during the course of a routine port access or for surveillance. Mark date of testing on isolator activity sheet. Newly constructed isolators will be tested 1 week after assembly and 1 week after mice are transfered in. Allow up to 5 days after testing for cultures to be negative before moving mice into a new isolator. **Note: when samples are submitted, please include a swab taken from mice known to be colonized or those from a conventional mouse room. Do not specify which swab this was when samples are dropped off.**


### 5A Sampling Isolators
- [ ] Sterilize external surface of MST using ExSpore Prepared as per Exspore SOP (1:4:1 base:water:activator made >15min <24h ahead of time) and transfer into isolator to be tested allowing for at least 45 minutes contact time as per *Entering Supplies SOP*.
- [ ] Dry any remaining sterilant from MST and open packaging.
- [ ] Swab any surfaces which mice may forseeably contact including inside of cages, wire racks, and fecal collection containers.
- [ ] Swab mold trap (small cup containing water and food which may be left in isolator to test for mold contamination).
- [ ] Return swab to transport media
- [ ] Add ~ 0.5 mL drinking water from a water bottle to the transport media
- [ ] If isolator contains animals: use forceps to collect 3 fecal pellets and place in transport media. Ideally fecal pellets will be collected from multiple cages.
- [ ] Close MST and remove from isolator. Store at 4˚C until testing.


### 5B Culture Testing
- [ ] On lab bench working by flame (or in BSC) vortex MST to homogenize fecal samples into transport media. Clean work space with 70% ethanol before use.
- [ ] Remove one swab and dab inoculum on to TSB plate and BHI CHVR plate. Use four quadrant streak method to spread swab contents over plate.
- [ ] Remove second swab and dab inocolum into two different tubes of 5mL BHI CHVR liquid media in 15mL tube
- [ ] Transfer TSB plate and one liquid culture to 37˚C aerobic incubator. Incubate liquid culture with shaking
- [ ] Transfer BHI CHVR plate and second liquid culture to 37˚C anaerobic incubator.
- [ ] Proceed to qPCR testing

### 5C qPCR Testing
- [ ] Transfer 200 ul of liquid contents of MST into bead beating tube.
- [ ] Follow [protocol for DNA extraction using zymo kit](https://github.com/bisanzlab/AmpliconSeq/blob/master/wetlab_protocols/1_DNAExtraction.md)
- [ ] Using eluted DNA set up qPCR rxns in 384 well plates according to volumes listed in Table 5.2
- [ ] Run qPCR with detection set for FAM probe according to parameters in Table 5.3.


**Table 5.2: qPCR reaction volumes**
|Component|[stock]|µL/rxn|[final]|
|-|-|-|-|
|iTaq Probes Supermix|2X|5|1X|
|10X assay mix|2µM|1|200nM|
|Water|-|2|-|
|DNA template|variable|2|varable|


**Table 5.3: qPCR Cycling Parameters**
Cycle |	Temperature (˚C)  | Time
------|-------------------|------
Initial Denaturation   |	95	| 5min
||
40 cycles:
Denature | 95˚C | 5 sec
Anneal/Extend | 60˚C	| 15 sec
||
Hold	| 4˚C	Hold | 0 sec


## Expected Results:

**Culture:** It is expected that no colonies will form. Most detection should be spotted within ~2 days; however, give up to 5 days for contamination to become visible. If plates drying out becomes an issue, place them in a plastic bag with a wet papertowel for extended incubation. The broth culture should not become turbid.

**qPCR:** Quantitative comparison of germ-free mice against negative extraction controls should be conducted. It is expected that germ-free mice should have a Ct no more than 1 cycle greater than negative controls. The Positive control should beging to amplify between cycles 10-15. **Note: all DNA extraction/PCR reagents contain trace microbial DNA, and as such, amplification is always expected in the cycle range ~33-38. If samples do not amplify in this range, it is an indication of carry over ethanol from reaction. Sample should be diluted 100x and re-assayed.

**In the event of positive test:** Retest immediately and/or send culture for Sanger 16S rRNA sequencing or MALDI-TOF. 
