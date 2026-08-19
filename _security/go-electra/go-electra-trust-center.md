---
certifications: []
description: Electra runs a real, publicly linked trust centre. It is the "Security" entry in the site footer on www.go-electra.com and it resolves to a Vanta-hosted trust report on Electra's own subdomain. The automated probe (0-working/probe-security-programs.py) recorded trust=none because it requires trust/compliance keywords in the served body, and Vanta serves a 4.8KB HTML shell that renders its content client-side from a signed bundle — so the presence of the trust centre is verified, but its contents are not readable anonymously.
kind: trust-center
layout: security
name: Go Electra Trust Center
name_suffix: Trust Center
overview: Electra maintains a public trust center covering its security and compliance posture.
provider_name: Electra
provider_slug: go-electra
slug: go-electra-trust-center
source_filename: go-electra-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: searched\nprobe: true\nurl: https://trust.go-electra.com/\ndescription: >-\n  Electra runs a real, publicly linked trust centre. It is the \"Security\" entry\n  in the site footer on www.go-electra.com and it resolves to a Vanta-hosted\n  trust report on Electra's own subdomain. The automated probe\n  (0-working/probe-security-programs.py) recorded trust=none because it requires\n  trust/compliance keywords in the served body, and Vanta serves a 4.8KB HTML\n  shell that renders its content client-side from a signed bundle — so the\n  presence of the trust centre is verified, but its contents are not readable\n  anonymously.\nplatform: Vanta\nplatform_evidence:\n  slug_id: 29bokoh51ag58ypkefl6z3\n  og_image: https://app.eu.vanta.com/doc?s=telu03zq9am1bikvdmnesj\n  bundle_host: assets.vanta.com\n  region: eu\ncertifications: []\ncertifications_note: >-\n  NO certification is asserted. The page title is \"Electra Trust Center\" and\n  nothing else\
  \ in the served markup names ISO 27001, SOC 2, PCI DSS, HIPAA,\n  FedRAMP or GDPR. Attempts to read the underlying report data anonymously all\n  failed: app.eu.vanta.com/api/trust/<slug>, app.eu.vanta.com/trust/<slug> and\n  app.vanta.com/api/trust/<slug> each returned the same HTML shell, and\n  app.eu.vanta.com/graphql rejected an anonymous query with HTTP 400 \"Missing\n  `signature` or `signedAt`\". Because no certification is readable, no\n  `Compliance` pointer is emitted in apis.yml.\nevidence:\n- source: https://www.go-electra.com/en/\n  kind: footer-link\n  http_status: 200\n  detail: >-\n    Footer anchor `<a href=\"https://trust.go-electra.com/\" ... >Security</a>`\n    in the legal/help column, alongside Assistance, Contact, General T&C,\n    Privacy Policy and Ethics.\n  fetched: '2026-08-17'\n- source: https://trust.go-electra.com/\n  kind: trust-center\n  http_status: 200\n  content_type: text/html\n  detail: >-\n    4,866-byte Vanta trust-report shell; <title>Electra Trust\
  \ Center</title>;\n    data-slugid=\"29bokoh51ag58ypkefl6z3\".\n  fetched: '2026-08-17'\n- source: https://app.eu.vanta.com/graphql\n  kind: negative\n  http_status: 400\n  detail: 'Anonymous query rejected: Missing `signature` or `signedAt`.'\n  fetched: '2026-08-17'\ngaps:\n- >-\n  No vulnerability disclosure or responsible-disclosure policy is published.\n  /.well-known/security.txt returned 404 on go-electra.com,\n  backend.go-electra.com and ocpi.go-electra.com. The only reporting channel\n  Electra publishes is its ethics/whistleblowing page\n  (https://www.go-electra.com/en/whistleblowing-and-grievance/, ethics@go-electra.com,\n  anonymous Google Forms, postal mail to VP Legal), which is explicitly scoped to\n  the Code of Conduct, corruption and harassment — it names no security contact\n  and no bug bounty. Consequently no `Security` /\n  `VulnerabilityDisclosure` artifact or pointer is emitted, and the\n  security_disclosure check is a genuine miss rather than an unrecorded one.\n\
  - >-\n  A security researcher who found a flaw in the OCPI surface has no published\n  address to send it to. Adding a security.txt on go-electra.com and\n  ocpi.go-electra.com, and surfacing the disclosure policy that almost certainly\n  already exists inside the Vanta trust centre, is the single cheapest fix on\n  this profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-electra/refs/heads/main/security/go-electra-trust-center.yml
summary_line: trust center published
tags:
- Company
- Climate Tech
- EV Charging
- Energy
- Mobility
- OCPI
- Roaming
- Charge Point Operator
- Electric Vehicles
- Fast Charging
- Charging Sessions
- Tariffs
- Electrification
- France
- Europe
trust_url: https://trust.go-electra.com/
---
