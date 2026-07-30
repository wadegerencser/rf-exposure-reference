# RF Exposure: Why the Numbers Matter

An engineering reference on how RF exposure is measured, regulated, and certified. SAR, MPE, EIRP,
antenna gain, duty cycle, near field versus far field, and what published separation distances
actually mean.

## Read it now, nothing to install

| How | Where |
|---|---|
| **Open in a browser (recommended)** | **https://wadegerencser.github.io/rf-exposure-reference/** |
| Download the PDF | [RF-Exposure-Reference.pdf](RF-Exposure-Reference.pdf) (33 pages) |
| Run the local copy | `git clone https://github.com/wadegerencser/rf-exposure-reference.git` then open `index.html` |

The browser is the runtime. It is one self contained HTML file with no build step, no dependencies,
and no tracking. It works on a phone.

## What is in it

- **Part 1** Executive summary, including why this was written
- **Part 2** RF physics, plus a live calculator with sliders for power, antenna gain, distance, and
  duty cycle that computes power density and percent of the FCC limit
- **Part 3** Regulatory and standards bodies, and why national numbers differ
- **Part 4** Device reference table, filterable, organized by which compliance path applies
- **Part 5** Access point engineering, including the 6 GHz LPI, SP, VLP, and GVP power regimes
- **Part 6** Scientific literature and agency positions, split into established, required by
  regulation, and open or contested, with a dedicated section on reproductive outcomes and
  offspring sex ratio
- **Part 7** Putting RF into perspective, and claims versus what the record supports

## Scope

This explains measurement, regulation, and certification. It is not medical advice and it does not
offer a health risk estimate. Calculations use a free space far field model, which is not valid at
contact distance, and near field cases are flagged in the charts as illustrations of scale rather
than compliance figures. Device table values are class level orientation drawn from regulatory
ceilings, not per model certified results. For any specific device, the authoritative sources are
its FCC ID exhibit and the vendor regulatory guide.

## Primary sources

47 CFR 1.1307, 1.1310, 2.1091, 2.1093, 15.407; FCC OET Bulletin 65; ICNIRP 2020; IEEE C95.1-2019;
Health Canada Safety Code 6; ISED RSS-102; IEC 62209-1528 and 62232; IARC Monograph Vol. 102;
NTP Technical Reports 595 and 596; Baste et al. 2008 (PMID 18415687); Tong et al. 2013
(PMID 23441458); Cordelli et al. 2023 (PMID 37729852). Full list in Part 7.
