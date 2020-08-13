# fedex-ras

Fedex Remote Areas List

The JSON file is created from the Fedex International Out-of-delivery-area And Out-of-pickup-area Surcharges List

Current version is from the Jul 20, 2020 PDF https://www.fedex.com/content/dam/fedex/us-united-states/services/Zipcodes_OPA_ODA.pdf

## Objectives

1. Preserve leading zeros
1. Expand ranges, so `0010 - 0012` actually yields 3 items: `0010`, `0011` and `0012`
1. Key by ISO 3166-1 alpha-2 code
1. Fix errors in the PDF published by Fedex (e.g. Missing "Brazil" heading) 
1. Distinguish between remote areas that incur surcharges for `pick_up_and_delivery`, `pick_up_only` or `delivery_only`