---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: calysta.com
  spf: true
hosts:
- cert_expires: Sep 13 08:14:17 2026 GMT
  host: calysta.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calysta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calysta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Calysta
provider_slug: calysta
slug: calysta-domain-security
source_filename: calysta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calysta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:14:17 2026 GMT\n  hsts: false\ndomains:\n- domain: calysta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calysta/refs/heads/main/security/calysta-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Cellular Agriculture
- Fermentation
- Alternative Protein
- Animal Feed
- Aquaculture
- Food Ingredients
- Sustainability
- Pet Nutrition
---
