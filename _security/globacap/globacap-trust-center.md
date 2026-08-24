---
certifications: []
description: ''
kind: trust-center
layout: security
name: Globacap Trust Center
name_suffix: Trust Center
overview: Globacap maintains a public trust center covering its security and compliance posture.
provider_name: Globacap
provider_slug: globacap
slug: globacap-trust-center
source_filename: globacap-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: https://trust.globacap.com/\ntrust_center:\n  present: true\n  url: https://trust.globacap.com/\n  vendor: Vanta\n  vendor_evidence: >-\n    The page is served from Vanta''s trust-report application (assets.vanta.com\n    bundles, data-slugid=\"eda5lcia16p2rw5tcp3wi\") and sets\n    <link rel=\"canonical\" href=\"https://trust.globacap.com\">, which is only emitted\n    for a configured custom trust-center domain.\n  http_status: 200\ncertifications: []\ncertifications_note: >-\n  NONE RECORDED — and that is a measurement, not an omission. The trust center is a\n  client-side React single-page app: the anonymous HTML response is a 4,261-byte\n  shell containing no certification names, and the same shell is returned for every\n  path on the host. Vanta''s data APIs (api.vanta.com/v1/trust-pages/<slug>,\n  /v1/trust-center/<slug>) return HTTP 401 anonymously and its GraphQL endpoint has\n  been retired (HTTP 410). A targeted web\
  \ search for Globacap SOC 2 / ISO 27001\n  returned no primary source. No certification is asserted here because none could\n  be read from a public, machine-readable surface. Do NOT emit a Compliance pointer\n  from this file.\nsubprocessors_page: null\nrequires_nda: unknown\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/globacap/refs/heads/main/security/globacap-trust-center.yml
summary_line: trust center published
tags:
- Company
- Private Capital Markets
- Capital Markets
- Securities
- Financial Services
- Fintech
- Tokenization
- Share Register
- Secondary Markets
- United Kingdom
trust_url: ''
---
