---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: allenapharma.com
  spf: true
hosts:
- cert_expires: Sep  5 06:24:39 2026 GMT
  host: allenapharma.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Allena Pharmaceuticals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allena Pharmaceuticals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Allena Pharmaceuticals
provider_slug: allena-pharmaceuticals
slug: allena-pharmaceuticals-domain-security
source_filename: allena-pharmaceuticals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: allenapharma.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  5 06:24:39 2026 GMT\n  hsts: null\ndomains:\n- domain: allenapharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allena-pharmaceuticals/refs/heads/main/security/allena-pharmaceuticals-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Biotech
- Pharmaceuticals
- Life Sciences
- Drug Development
- Healthcare
---
