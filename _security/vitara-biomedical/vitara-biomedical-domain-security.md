---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vitara.com
  spf: true
hosts:
- cert_expires: Aug 30 07:26:30 2026 GMT
  host: vitara.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vitara Biomedical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vitara Biomedical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Vitara Biomedical
provider_slug: vitara-biomedical
slug: vitara-biomedical-domain-security
source_filename: vitara-biomedical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vitara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 07:26:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: vitara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitara-biomedical/refs/heads/main/security/vitara-biomedical-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Life Sciences
- Medical Devices
- Neonatal Care
- Healthcare
- Biomedical
- Medical Technology
---
