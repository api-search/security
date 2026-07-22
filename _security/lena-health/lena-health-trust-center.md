---
certifications:
- SOC 2 Type II
- HIPAA
description: ''
kind: trust-center
layout: security
name: Lena Health Trust Center
name_suffix: Trust Center
overview: Lena Health maintains a public trust center documenting SOC 2 Type II and HIPAA compliance.
provider_name: Lena Health
provider_slug: lena-health
slug: lena-health-trust-center
source_filename: lena-health-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: true\nsource: https://lena.io/llms.txt\nurl: https://trust.lenaconnect.com/\ncertifications:\n- SOC 2 Type II\n- HIPAA\nnotes: >-\n  The trust center is hosted off the primary marketing domain at\n  trust.lenaconnect.com and is client-side rendered, so no certification names are\n  present in its server-returned HTML (HTTP 200, 4,239 bytes, JS shell). The\n  certification names recorded here are taken verbatim from Lena Health's own\n  first-party sources on lena.io, which also publish the trust center URL. Note\n  that lena.io is a single-page app that returns its index.html for every unknown\n  path, so an automated probe of https://lena.io/trust returns HTTP 200 with the\n  homepage; that soft-404 is not a real trust-center page and has been corrected\n  here.\nevidence:\n- source: https://lena.io/llms.txt\n  kind: llms.txt\n  quote: 'Compliance & Security: HIPAA Compliant; SOC 2 Type II Certified; Trust Center:\n    https://trust.lenaconnect.com/'\n\
  - source: https://lena.io/\n  kind: meta-description\n  quote: SOC 2 Type II and HIPAA compliant.\n- source: https://lena.io/\n  kind: schema.org FAQPage\n  quote: Yes, Lena Health is both HIPAA compliant and SOC 2 Type II certified, ensuring\n    the highest standards of data security and privacy for healthcare organizations.\n- source: https://trust.lenaconnect.com/\n  kind: trust-center\n  status: 200\n  title: Lena Health Trust Center\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lena-health/refs/heads/main/security/lena-health-trust-center.yml
summary_line: SOC 2 Type II, HIPAA
tags:
- Company
- Healthcare
- Health Care Coordination
- Care Navigation
- Artificial Intelligence
- Patient Engagement
- Chronic Care Management
- Health Plans
- Digital Health
- HIPAA
trust_url: https://trust.lenaconnect.com/
---
