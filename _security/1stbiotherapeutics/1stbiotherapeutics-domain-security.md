---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1stbio.com
  spf: true
hosts:
- cert_expires: Oct  3 02:44:07 2026 GMT
  host: www.1stbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1Stbiotherapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1ST Biotherapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 1ST Biotherapeutics
provider_slug: 1stbiotherapeutics
slug: 1stbiotherapeutics-domain-security
source_filename: 1stbiotherapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1stbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:44:07 2026 GMT\n  hsts: false\ndomains:\n- domain: 1stbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1stbiotherapeutics/refs/heads/main/security/1stbiotherapeutics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Life Sciences
- Healthcare
- Oncology
- Neurodegenerative Disease
- Rare Disease
- South Korea
---
