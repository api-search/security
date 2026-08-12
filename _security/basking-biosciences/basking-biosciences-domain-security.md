---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: baskingbiosciences.com
  spf: true
hosts:
- cert_expires: Oct 23 01:22:22 2026 GMT
  host: www.baskingbiosciences.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basking Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basking Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Basking Biosciences
provider_slug: basking-biosciences
slug: basking-biosciences-domain-security
source_filename: basking-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baskingbiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 01:22:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baskingbiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basking-biosciences/refs/heads/main/security/basking-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech Therapeutics
- Biopharmaceutical
- Clinical Stage
- Stroke
- Thrombosis
- Drug Development
- Life Sciences
---
