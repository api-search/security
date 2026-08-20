---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: procyrion.com
  spf: true
hosts:
- cert_expires: Oct  3 21:44:41 2026 GMT
  host: www.procyrion.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Procyrion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procyrion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Procyrion
provider_slug: procyrion
slug: procyrion-domain-security
source_filename: procyrion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.procyrion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:44:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: procyrion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procyrion/refs/heads/main/security/procyrion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Medical Devices
- Healthcare
- Cardiology
- Heart Failure
- Mechanical Circulatory Support
- Medical Technology
- Clinical Trials
---
