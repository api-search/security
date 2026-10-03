---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brainever.fr
  spf: true
hosts:
- cert_expires: Nov 12 06:47:31 2026 GMT
  host: brainever.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brainever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brainever, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Brainever
provider_slug: brainever
slug: brainever-domain-security
source_filename: brainever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brainever.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 06:47:31 2026 GMT\n  hsts: false\ndomains:\n- domain: brainever.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainever/refs/heads/main/security/brainever-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biopharma
- Neurodegenerative
- Homeoprotein
- ALS
- Parkinson
---
