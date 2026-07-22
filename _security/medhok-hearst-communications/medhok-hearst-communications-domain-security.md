---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mhk.com
  spf: true
hosts:
- cert_expires: Sep 14 06:31:39 2026 GMT
  host: mhk.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medhok Hearst Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedHOK (Hearst Communications), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MedHOK (Hearst Communications)
provider_slug: medhok-hearst-communications
slug: medhok-hearst-communications-domain-security
source_filename: medhok-hearst-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mhk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:31:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mhk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medhok-hearst-communications/refs/heads/main/security/medhok-hearst-communications-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Plans
- Payer
- Care Management
- Utilization Management
- Interoperability
- FHIR
- Compliance
---
