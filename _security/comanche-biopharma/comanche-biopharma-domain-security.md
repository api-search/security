---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: comanchebiopharma.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: comanchebiopharma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comanche Biopharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comanche Biopharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Comanche Biopharma
provider_slug: comanche-biopharma
slug: comanche-biopharma-domain-security
source_filename: comanche-biopharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comanchebiopharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: comanchebiopharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comanche-biopharma/refs/heads/main/security/comanche-biopharma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Life Sciences
- Biopharmaceutical
- Biotechnology
- Maternal Health
- Preeclampsia
- siRNA Therapeutics
- Drug Development
---
