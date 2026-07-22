---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axsome.com
  spf: true
hosts:
- cert_expires: Sep 29 21:57:40 2026 GMT
  host: www.axsome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axsome Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axsome Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axsome Therapeutics
provider_slug: axsome-therapeutics
slug: axsome-therapeutics-domain-security
source_filename: axsome-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axsome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:57:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axsome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axsome-therapeutics/refs/heads/main/security/axsome-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Biopharmaceuticals
- Biotechnology
- Pharmaceuticals
- Healthcare
- Life Sciences
- Neuroscience
- Central Nervous System
- Depression
- Migraine
- Narcolepsy
- Alzheimers Disease Agitation
- Fibromyalgia
- Smoking Cessation
- Clinical Pipeline
- FDA Approved
---
