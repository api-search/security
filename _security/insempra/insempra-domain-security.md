---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: insempra.bio
  spf: true
hosts:
- cert_expires: Sep  6 18:25:11 2026 GMT
  host: insempra.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insempra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insempra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Insempra
provider_slug: insempra
slug: insempra-domain-security
source_filename: insempra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insempra.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:25:11 2026 GMT\n  hsts: false\ndomains:\n- domain: insempra.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insempra/refs/heads/main/security/insempra-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotech
- Precision Fermentation
- Synthetic Biology
- Sustainability
- Bio-based Materials
- Ingredients
---
