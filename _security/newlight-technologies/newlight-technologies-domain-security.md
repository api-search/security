---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: newlight.com
  spf: false
hosts:
- cert_expires: Oct  4 19:30:56 2026 GMT
  host: www.newlight.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newlight Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newlight Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Newlight Technologies
provider_slug: newlight-technologies
slug: newlight-technologies-domain-security
source_filename: newlight-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.newlight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:30:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: newlight.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newlight-technologies/refs/heads/main/security/newlight-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Biomaterials
- Materials Science
- Sustainability
- Carbon Capture
- Manufacturing
- Bioplastics
- Climate Technology
- Consumer Products
---
