---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ultimagenomics.com
  spf: true
hosts:
- cert_expires: Oct  7 14:53:48 2026 GMT
  host: www.ultimagenomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ultima Genomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ultima Genomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ultima Genomics
provider_slug: ultima-genomics
slug: ultima-genomics-domain-security
source_filename: ultima-genomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ultimagenomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ultimagenomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultima-genomics/refs/heads/main/security/ultima-genomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Genomics
- DNA Sequencing
- Bioinformatics
- Life Sciences
- Sequencing
- AWS HealthOmics
---
