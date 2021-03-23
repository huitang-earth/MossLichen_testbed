00_README
This dataset presents data for "Contrasting drivers of community-level trait variation for vascular plants, lichens, and bryophytes across an elevational gradient, Roos & Van Zuijlen et al. 2019, Functional Ecology". The set contains data on vascular plant, lichen, and bryophyte cover and functional traits across an elevational gradient in Finse, southern Norway (2019-08-30)

The dataset includes four files: 
1. Gradient_traits.txt includes trait and abundance data for all primary producer groups (vascular plants, lichens and bryophytes), except pH and bryophyte-SLA.
2. Gradient_bryoSLA.txt includes SLA and abundance data for bryophytes only.
3. Gradient_pH.txt includes pH and abundance data for all three primary producer groups.
4. Species_names.txt includes a list of all species names and used abbreviations.

The traits included in the three files are:
N		Nitrogen concentration (%); all groups
P		Phosphorus concentration (%); all groups
NP		Nitrogen to Phosphorus ratio; all groups
pH		pH; all groups
SLA		Specific Leaf Area (mm2 mg-1); vascular plants and bryophytes
STA		Specific Thallus Area (mm2 mg-1); lichens
LDMC		Leaf Dry Matter Content (g g-1); vascular plants
WHC		Water Holding Capacity (g g-1); bryophytes
WHCa		Water Holding Capacity per thallus area (mg mm-2)

Explanation of the column names:
elevation		Elevation in m above sea level
plot			Plot number (1-5)
site.plot	Elevation and plot number combined in one variable; 1120p1 stands for plot 1 at 1120 m a.s.l.
group	Primary producer group: bryo=bryophytes, lich=lichens, vasc=vascular plants
genus			Genus name of the species (in full)
species			Species code (abbreviation, see Species_names.txt)
cover.original			Cover estimate as measured in the field, in % of 1m2 (plot size)
cover.adjusted	Cover estimate as used in the community-level calculations; set to 0 if no trait measurements were available
rel.cover.adjusted	Relative cover per species per group per plot; calculated from the the sum of cover.adjusted
N, P, NP, pH, SLA, STA, LDMC, WHC, WHCa
	Trait values per species per plot, based on individual measurements or elevation averages if plot-level measurements were not available
fixedN, fixedP, fixedNP, fixedpH, fixedSLA, fixedSTA, fixedLDMC, fixedWHC, fixedWHCa
	Trait averages per species, independent of plot or site (“fixed”)
rel.N, rel.P, rel.NP, rel.pH, rel.SLA, rel.STA, rel.LDMC, rel.WHC, rel.WHCa
	Relative trait value; trait value multiplied by the relative cover per species per group per plot
rel.fixedN, rel.fixedP, rel.fixedNP, rel.fixedpH, rel.fixedSLA, rel.fixedSTA, rel.fixedLDMC, rel.fixedWHC, rel.fixedWHCa
	Relative fixed trait value; trait average per species multiplied by the relative cover per species per group per plot 

The community.weighted mean is calculated as the sum of the relative trait values for each group for each plot. For details on the trait measurements and community-weighted mean calculations, see our paper Roos et al. 2019 in Functional Ecology.
