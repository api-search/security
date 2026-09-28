---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bioprotonics.com
  spf: true
hosts:
- cert_expires: Nov 17 11:06:38 2026 GMT
  host: www.bioprotonics.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioprotonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioProtonics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BioProtonics
provider_slug: bioprotonics
slug: bioprotonics-domain-security
source_filename: bioprotonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioprotonics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 11:06:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bioprotonics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioprotonics/refs/heads/main/security/bioprotonics-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Medical Imaging
- Diagnostics
- AI
- Healthcare
---
