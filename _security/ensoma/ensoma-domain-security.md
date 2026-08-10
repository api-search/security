---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ensoma.com
  spf: true
hosts:
- cert_expires: Oct  4 21:26:44 2026 GMT
  host: ensoma.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ensoma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ensoma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ensoma
provider_slug: ensoma
slug: ensoma-domain-security
source_filename: ensoma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ensoma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:26:44 2026 GMT\n  hsts: null\ndomains:\n- domain: ensoma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ensoma/refs/heads/main/security/ensoma-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Genomic Medicine
- Gene Therapy
- Cell Therapy
- Life Sciences
- Healthcare
- Bioinformatics
- Private Company
---
