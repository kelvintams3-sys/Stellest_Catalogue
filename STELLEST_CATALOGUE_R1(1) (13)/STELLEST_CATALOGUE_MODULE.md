# Stellest Catalogue

## Purpose

Touch-first customer consultation catalogue that compares, builds and prints quotations for:

- STELLEST
- STELLEST 2.0

The application is a standalone static website. It does not alter or depend on ZIC.

## Design reference

The interface follows the approved ZIC design language:

- iPad-first portrait layout
- deep navy typography and navigation
- rounded white cards on a pale-grey background
- pale-blue Grand Total panels
- large touch targets and concise customer-facing copy
- prominent product identity in the summary and printout

## Product comparison

| Product | Technology | Lenslets | Rings | Customer-facing efficacy |
| --- | --- | ---: | ---: | --- |
| STELLEST | H.A.L.T. | 1,021 | 11 | 67% slower myopia progression versus single-vision lenses. |
| STELLEST 2.0 | H.A.L.T. MAX | 1,190 | 12 | Approximately 47% less eye-length growth versus STELLEST. |

The STELLEST 2.0 efficacy line links to:

https://doi.org/10.1167/tvst.14.11.9

## Prices

| Product | Crizal Rock | Crizal Prevencia |
| --- | ---: | ---: |
| STELLEST | RM1,300 | RM1,400 |
| STELLEST 2.0 | RM1,700 | RM1,800 |

Prices are per pair.

## Interaction rules

- The catalogue opens directly on the two-product comparison.
- A bright, undimmed child hero image appears above the comparison with the tagline “Clear vision today. A brighter future tomorrow.”
- STELLEST and STELLEST 2.0 titles share one horizontal baseline.
- Lenslets, concentric rings, lenslet design, efficacy and coating sections align across both product columns on iPad.
- All four lens-and-coating prices are selectable on the comparison page; there is no separate configuration page.
- Frame and Biometry follow-up controls appear on Review Summary, not on the comparison page.
- Review Summary uses one consistent typographic hierarchy for section labels, item names and amounts.
- Review Summary uses compact card spacing; the main section text is larger while the two follow-up rows are deliberately quieter.
- Lens coating, frame and follow-up line-item prices use the same font size, weight and colour on Review Summary.
- Frame is optional and omitted when blank.
- Pressing and holding Frame toggles its entered amount to COMPLIMENTARY; the original amount remains visible with a strikethrough and contributes RM0 to the Grand Total.
- Biometry Follow-up 1 is RM120.
- Biometry Follow-up 2 is RM120.
- Each follow-up can be included or excluded independently.
- Pressing and holding the Biometry follow-up title toggles both follow-ups between their normal price and COMPLIMENTARY; RM120 remains visible with a strikethrough.
- Complimentary follow-ups contribute RM0 to the Grand Total.
- The summary updates immediately.

## Print output

- The quotation remains portrait. The guarantee appears landscape but is rotated inside the printer's physical 40 × 60 mm label size.
- Printed labels use a positive black Essilor logo on white. The quotation uses a slightly smaller product name and price details with more spacing between the logo, product and item rows.
- Complimentary frame and follow-up entries retain their struck-through original prices on the printout without printing the word COMPLIMENTARY.
- The separate guarantee label reads: “6-Month Prescription Change Guarantee — For prescription increase by 0.75D or more within 6 months, lenses will be replaced at no charge.”
- The guarantee sentence uses smaller supporting text than the guarantee title.
- A third landscape booklet label appears below the first two labels and is reached by scrolling down; it is rotated inside the physical 40 × 60 mm label size.
- The booklet label includes unticked “Follow-up 1” and “Follow-up 2” boxes, with blank space for handwritten follow-up dates and no printed date lines.
- It states that further biometry follow-ups are RM120 per visit and repeats the six-month guarantee wording.
- The booklet guarantee title and supporting sentence are clearly separated, with slightly larger supporting text for readability.
- Browser printing is omitted.
- Supports AIMO D520BT-Z Bluetooth printing through Bluefy/WebBLE using the same FF00/FF02/FF03 channel pattern as ZIC.
- The print panel shows connecting, sending, success and failure status without closing after a print.

## Files

    index.html
    assets/
      essilor-logo.png
      stellest-hero.png
    trigger/
      deploy.txt

The site is self-contained apart from the external clinical-study link.

## Release checks

- The catalogue opens on the comparison page with no intro or configuration step.
- Both product titles and all four lens-and-coating choices display together.
- Coating prices match the 2026 list.
- Frame amount is included only when entered; a complimentary frame keeps its original amount struck through and restores that amount when toggled back.
- Follow-up totals calculate correctly in paid and complimentary states.
- STELLEST 2.0 study link opens the peer-reviewed paper.
- Summary and print label preserve the selected options.
- All D520BT-Z output remains physically 40 × 60 mm. The guarantee and booklet artwork, including the bitmap logo, is rotated 90° within the vertical stock for landscape printing.
- No customer or patient data is stored.

## Current release

2026-09-28-r1.22
