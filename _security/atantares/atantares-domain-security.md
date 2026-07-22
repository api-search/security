---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: atantares.com
  spf: true
hosts:
- cert_expires: Aug 22 15:12:02 2026 GMT
  host: atantares.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atantares Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for atantares, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: atantares
provider_slug: atantares
slug: atantares-domain-security
source_filename: atantares-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: atantares.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:12:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: atantares.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atantares/refs/heads/main/security/atantares-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Biotechnology
- Synthetic Biology
- DNA Synthesis
- Genomics
- Life Sciences
- Semiconductors
- Gene Sequencing
---
