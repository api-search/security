---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: absology.co.kr
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.absology.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Absology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Absology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Absology
provider_slug: absology
slug: absology-domain-security
source_filename: absology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.absology.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: absology.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/absology/refs/heads/main/security/absology-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Health Care
- Medical Devices
- Diagnostics
- In-Vitro Diagnostics
- Point Of Care
- Laboratory
- South Korea
---
