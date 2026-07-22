---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: whitehouse.gov
  spf: true
hosts:
- cert_expires: Sep  1 19:58:03 2026 GMT
  host: www.whitehouse.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Council On Environmental Quality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Council on Environmental Quality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Council on Environmental Quality
provider_slug: council-on-environmental-quality
slug: council-on-environmental-quality-domain-security
source_filename: council-on-environmental-quality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.whitehouse.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 19:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whitehouse.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/council-on-environmental-quality/refs/heads/main/security/council-on-environmental-quality-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CEQ
- Climate
- Environment
- Environmental Justice
- Environmental Policy
- Executive Office of the President
- Federal Government
- Government
- NEPA
- Permitting
- Public Data
- White House
---
