---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3tbiosciences.com
  spf: true
hosts:
- cert_expires: Sep 23 09:41:47 2026 GMT
  host: 3tbiosciences.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 3T Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3T Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3T Biosciences
provider_slug: 3t-biosciences
slug: 3t-biosciences-domain-security
source_filename: 3t-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 3tbiosciences.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:41:47 2026 GMT\n  hsts: false\ndomains:\n- domain: 3tbiosciences.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3t-biosciences/refs/heads/main/security/3t-biosciences-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotech
- Immunotherapy
- Oncology
- TCR Therapeutics
- Cell Therapy
- Drug Discovery
- Machine Learning
---
