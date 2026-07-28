---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nationalgrid.co.uk
  spf: true
hosts:
- cert_expires: Aug 29 02:28:57 2026 GMT
  host: www.nationalgrid.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:51:30 2026 GMT
  host: connecteddata.nationalgrid.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 04:01:44 2026 GMT
  host: dso.nationalgrid.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Grid Electricity Distribution Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Grid Electricity Distribution, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Grid Electricity Distribution
provider_slug: national-grid-electricity-distribution
slug: national-grid-electricity-distribution-domain-security
source_filename: national-grid-electricity-distribution-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nationalgrid.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:28:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: connecteddata.nationalgrid.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dso.nationalgrid.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 04:01:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nationalgrid.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-grid-electricity-distribution/refs/heads/main/security/national-grid-electricity-distribution-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- DER
- Flexibility
- Renewables
---
