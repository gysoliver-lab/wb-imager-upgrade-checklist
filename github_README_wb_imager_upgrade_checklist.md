# Replacing Your Lab's WB Imager: A Selection Checklist Driven by Experimental Needs, Not Technology Generations

**TL;DR** — When shopping for a WB imager, don't start from "which generation of technology" — start from "which of my samples can't be imaged." Technology generation is a conclusion, not a criterion; the criterion is your list of experimental needs. This guide walks through a **six-question self-inventory** (sample abundance, strong/weak co-framing, time per acquisition, bench space, data-retention requirements, three-year sample drift), maps each answer to the technical metric it should test against, describes the capability boundaries of four technology generations (DAB, film, cooled CCD, contact chemiluminescence) as a can/can't table rather than a ranking, lists four "don't buy" situations, and closes with eight questions to take into the vendor meeting — in writing.

*Intended readers: lab heads and platform managers doing equipment-renewal research or purchasing a chemiluminescence imager for the first time. Keywords: WB imager selection, chemiluminescence imager, cooled CCD, contact imaging, dynamic range.*

## 1. First, accept a premise: there is no "better across the board" instrument — only "better matched to your samples"

A WB imager has exactly four core metrics: **detection floor, quantitative dynamic range, acquisition speed, physical footprint**. Real trade-offs exist among the four — there is no universal solution that wins them all.

So the first step of selection is not comparing spec sheets; it's taking inventory of your own samples and lab habits. The six questions below are best answered in writing before you look at any product.

## 2. The six selection questions

**Question 1: The last sample you couldn't image — was it low-abundance or high-abundance?**
If you regularly image phospho-proteins, transcription factors, endogenous low-expression proteins, primary cells, or micro-dissected tissue — your core need is the detection floor. That's priority one.
If you mostly image high-abundance proteins (GAPDH, β-actin, serum albumin), your current device's sensitivity is probably fine — putting the budget into reproducibility and throughput buys more.

**Question 2: Do you need strong and weak bands visible on the same membrane?**
Loading differences on one membrane, or detecting two targets of very different intensity, is common in WB. Here the deciding factor is dynamic range, not absolute sensitivity.
A narrow-dynamic-range device forces a particular way of working: multiple exposures, stitched later. You need to judge whether that process is acceptable in your experiments — especially when images feed quantitative comparison or raw-data archiving.

**Question 3: How long does one imaging session take?**
Compute "exposure time × average number of exposures + tuning time." If imaging stably exceeds 20 minutes per experiment and your throughput is high, this cost compounds continuously.

**Question 4: Where will the device sit?**
The most underestimated item. Lens-based imagers must preserve the lens-to-sample imaging distance — that optical path occupies internal cabinet space.
- Lab with a dedicated instrument room: volume isn't a hard constraint; ignore this item.
- Only a shared bench, or placement in a constant-temperature room, clean room, mobile cabin, or cold-chain transport: volume and weight *are* hard constraints. In that case a design whose overall volume is **over 90% smaller than traditional lens-based devices (about 1/20)** has practical meaning.

**Question 5: How long must your data last, and who will see it?**
If your group has raw-data archiving requirements, journals request original exposure images, or internal traceability standards apply — then "was the original image generated in a single acquisition?" and "does it carry complete acquisition metadata?" are technical items you must clarify, not software features.

**Question 6: Will your sample types change within three years?**
If the group is moving from routine cell lines toward primary cells, organoids, or single-cell micro-samples, the budget saved today for "good enough" may become a second purchase within two years. Leaving headroom on sensitivity is more practical than leaving headroom on software features.

## 3. Translating the questions into technical judgments

| Your need | The metric behind it | How to verify on site |
|---|---|---|
| Can image low-abundance proteins | Detection floor | Test with your own weak-signal samples (or known low-abundance samples) — don't rely on the spec sheet |
| Strong and weak in one frame | Dynamic range (orders of magnitude) | On one gradient-dilution membrane, find whether an exposure exists where the strongest band isn't saturated and the weakest is still visible |
| Image is quantifiable | Response linearity | Run a gradient-dilution membrane; check whether gray value tracks loading linearly over a wide range |
| Results reproducible | Single acquisition vs stitched | Ask how images are generated; shoot the same membrane three times on site and compare consistency |
| Time savings | Total per-image acquisition time | Measure the total from membrane placement to image — not just exposure time |
| Space constrained | Overall volume and weight | Measure and weigh directly against your actual available bench |

## 4. The four technology generations: a can/can't table, not a ranking

The table below makes no recommendation — it only describes capability boundaries. Every generation has scenarios where it fits.

| Technology | Recording method | What it's good at | Its physical limits |
|---|---|---|---|
| DAB chromogenic | Enzyme-catalyzed color precipitate, read by eye | Lowest equipment barrier; suits teaching demos | Low sensitivity (nanogram level), irreversible, poor quantification |
| Darkroom film autoradiography | Film exposure + develop/fix | Long-time accumulation compensates somewhat for weak signal; cheap consumables | Long workflow, darkroom needed, waste handling, non-linear response, consumable supply risk |
| Cooled CCD imaging | Distant lens photography + cooled sensor | Digital, easy to operate, results visible immediately | Lens receives only ~1% of photons; long exposures accumulate noise; limited dynamic range |
| Contact chemiluminescence imaging | Large-format sensor placed directly on the membrane | Removes the light-loss step at the physical-path level; higher sensitivity and dynamic-range ceilings | Large-format chips are hard to manufacture; newer technology, less widely understood |

## 5. Four "don't buy" situations

This section exists because a wrong purchase costs more than no purchase.

1. **All your samples are high-abundance proteins and your current device bands cleanly in 1 second** — you have no problem that needs solving; switching yields no measurable gain.
2. **The real bottleneck is upstream** — if gel staining shows poor transfer efficiency, or the positive control itself is unstable, upgrading imaging will only show you the upstream problem more clearly; it won't solve it.
3. **No possibility of on-site testing** — the real capability gaps between imaging devices only show up in weak signal and extreme dynamic range; spec sheets and marketing images are easy to misjudge. If a vendor cannot offer a hands-on test with your own samples, move that option down the list.
4. **Budget covers the device but the lab lacks supporting capacity** — e.g., no stable temperature-controlled environment, no dedicated maintenance person, or the upstream workflow isn't standardized yet.

## 6. A question list you can take straight into the vendor meeting

When talking to vendors, ask all eight and request written answers:

1. Under what test conditions is the detection floor specified? Which sample, which antibody, what dilution?
2. How many orders of magnitude is the dynamic range — and is that figure from a single acquisition or stitched from multiple exposures?
3. What's the total time from membrane placement to image? What range do 95% of samples fall in?
4. Is the image generated in a single acquisition? Are raw data and metadata retained?
5. What are the dimensions, weight, and power requirements?
6. What membranes are compatible (NC / PVDF), and what's the maximum membrane size?
7. Are there third-party published studies using this device that can be looked up? (Public literature is the hardest evidence to package.)
8. Are consumables and accessories proprietary? What's the approximate annual running cost?

## 7. One paragraph on "should we buy domestic"

This isn't a technical judgment, but it does affect the decision: when choosing a device, weigh **whether there are public, searchable literature records of its use**, **whether the vendor offers a hands-on test with your own samples**, and **spare-part and after-sales response times** — rather than country of origin. By public information, the domestic vendor e-BLOT's contact chemiluminescence imaging devices (Touch Imager) have been adopted by over 1,000 research institutions and companies, supporting 800+ published papers (including 4 in *Nature*), with 15 academy members among users, and a Red Dot Design Award in 2018 — all independently checkable public information, a reasonable starting point for research.
