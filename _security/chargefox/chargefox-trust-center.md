---
api_specs:
- filename: chargefox-fleets-api-openapi.yml
  format: yaml
  label: Chargefox Fleets API
  slug: chargefox-fleets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/openapi/chargefox-fleets-api-openapi.yml
certifications: []
description: 'Chargefox operates a public Trust Center at trust.chargefox.com, hosted on Vanta''s Australian instance (app.aus.vanta.com). Verified live on 2026-07-27: the page returns 200, carries `<link rel="canonical" href="https://trust.chargefox.com">`, the title "Chargefox Trust Center" and an og:description written by Chargefox describing the company and platform. The page body is rendered client-side from Vanta''s trust-report bundle, so the framework list, control set and document library are not readable anonymously by a non-JS client — they are not asserted here. No named certification could be verified without executing the page, and none is claimed in this artifact.'
kind: trust-center
layout: security
name: Chargefox Trust Center
name_suffix: Trust Center
overview: Chargefox maintains a public trust center covering its security and compliance posture.
provider_name: Chargefox
provider_slug: chargefox
slug: chargefox-trust-center
source_filename: chargefox-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nprobe: true\nurl: https://trust.chargefox.com/\ndescription: >-\n  Chargefox operates a public Trust Center at trust.chargefox.com, hosted on\n  Vanta's Australian instance (app.aus.vanta.com). Verified live on 2026-07-27:\n  the page returns 200, carries `<link rel=\"canonical\" href=\"https://trust.chargefox.com\">`,\n  the title \"Chargefox Trust Center\" and an og:description written by Chargefox\n  describing the company and platform. The page body is rendered client-side\n  from Vanta's trust-report bundle, so the framework list, control set and\n  document library are not readable anonymously by a non-JS client — they are\n  not asserted here. No named certification could be verified without executing\n  the page, and none is claimed in this artifact.\nplatform: Vanta\nplatform_region: app.aus.vanta.com (Vanta Australia)\nslug_id: cuvlumskotxw67nge444y3\ncertifications: []\ncertifications_note: >-\n  NOT verified. Chargefox's\
  \ specific frameworks (SOC 2, ISO 27001 or otherwise)\n  could not be confirmed from the anonymously reachable HTML, and no\n  certification claim appears on the marketing site, the developer docs or the\n  legal pages. A future round should re-check with a JS-capable fetch. Because\n  no certification is verified, no `Compliance` pointer is wired in apis.yml.\nevidence:\n  - source: https://trust.chargefox.com/\n    status: 200\n    kind: trust-center\n    keywords: [chargefox trust center, vanta, trust, security, compliance, automation]\n  - source: https://trust.chargefox.com/\n    kind: canonical-link\n    detail: 'rel=canonical points at https://trust.chargefox.com — a first-party, branded trust center rather than a shared Vanta page.'\nrelated:\n  domain_security: security/chargefox-domain-security.yml\n  vulnerability_disclosure: null\n  privacy_policy: https://www.chargefox.com/legal/privacy-policy\n  terms: https://www.chargefox.com/legal/terms-conditions\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargefox/refs/heads/main/security/chargefox-trust-center.yml
summary_line: trust center published
tags:
- Energy
- Australia
- EV Charging
- Electricity
- Utilities
- OCPI
- Charge Point Operator
- Roaming
- Fleets
- Mobility
- Charging Sessions
- Electrification
trust_url: https://trust.chargefox.com/
---
