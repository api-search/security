---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: orsobio.com
  spf: true
hosts:
- cert_expires: Sep  9 06:26:22 2026 GMT
  host: orsobio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orsobio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OrsoBio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: OrsoBio
provider_slug: orsobio
slug: orsobio-domain-security
source_filename: orsobio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orsobio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 06:26:22 2026 GMT\n  hsts: false\ndomains:\n- domain: orsobio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orsobio/refs/heads/main/security/orsobio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Metabolic Disease
- Obesity
- Clinical Trials
- Drug Development
- Healthcare
---
