---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: proscia.com
  spf: true
hosts:
- cert_expires: Sep 14 20:27:35 2026 GMT
  host: proscia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 14:13:30 2026 GMT
  host: cloud.proscia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Proscia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proscia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Proscia
provider_slug: proscia
slug: proscia-domain-security
source_filename: proscia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: proscia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:27:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.proscia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:13:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: proscia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proscia/refs/heads/main/security/proscia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Digital Pathology
- Pathology
- Life Sciences
- Precision Medicine
- Artificial Intelligence
- Medical Imaging
- Whole Slide Imaging
- Foundation Models
- Diagnostics
---
