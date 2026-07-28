---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ofgem.gov.uk
  spf: true
hosts:
- cert_expires: Oct  3 03:18:33 2026 GMT
  host: www.ofgem.gov.uk
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: epr.ofgem.gov.uk
  hsts: false
  https: true
  note: Electronic Public Register application. Probed manually 2026-07-27.
  tls_version: TLSv1.3
  tls_versions_supported:
  - TLSv1.3
  - TLSv1.2
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: epre-api.ofgem.gov.uk
  hsts: false
  https: true
  note: Electronic Public Register backend (Cognito sign-in plus the undocumented GraphQL endpoint). Probed manually 2026-07-27.
  tls_version: TLSv1.3
  tls_versions_supported:
  - TLSv1.3
  - TLSv1.2
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: rer.ofgem.gov.uk
  hsts: false
  https: true
  note: Renewable Electricity Register application. Probed manually 2026-07-27.
  tls_version: TLSv1.3
  tls_versions_supported:
  - TLSv1.3
  - TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ofgem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ofgem, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ofgem
provider_slug: ofgem
slug: ofgem-domain-security
source_filename: ofgem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts (0-working/probe-domain-security.py),\n  extended 2026-07-27 with manual TLS/HSTS probes of the three register hosts\nhosts:\n- host: www.ofgem.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: epr.ofgem.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  tls_versions_supported: [TLSv1.3, TLSv1.2]\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n  note: Electronic Public Register application. Probed manually 2026-07-27.\n- host: epre-api.ofgem.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  tls_versions_supported: [TLSv1.3, TLSv1.2]\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n  note: >-\n    Electronic Public Register backend (Cognito sign-in plus the undocumented\n    GraphQL endpoint). Probed manually 2026-07-27.\n- host: rer.ofgem.gov.uk\n  https: true\n  tls_version:\
  \ TLSv1.3\n  tls_versions_supported: [TLSv1.3, TLSv1.2]\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\n  note: Renewable Electricity Register application. Probed manually 2026-07-27.\ndomains:\n- domain: ofgem.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofgem/refs/heads/main/security/ofgem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Markets
- Regulator
- Smart Metering
- Open Data
- Energy Regulation
- Renewables
- Great Britain
---
