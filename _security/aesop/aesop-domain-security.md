---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aesoptek.com
  spf: true
hosts:
- cert_expires: Sep 25 23:14:54 2026 GMT
  host: aesoptek.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aesop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AESOP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AESOP
provider_slug: aesop
slug: aesop-domain-security
source_filename: aesop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aesoptek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:14:54 2026 GMT\n  hsts: false\ndomains:\n- domain: aesoptek.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aesop/refs/heads/main/security/aesop-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Artificial Intelligence
- Clinical Decision Support
- Medical Coding
- Diagnostics
- Medical AI
- Patient Safety
---
