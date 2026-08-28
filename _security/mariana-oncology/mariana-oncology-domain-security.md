---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marianaoncology.com
  spf: true
hosts:
- cert_expires: Oct 14 01:13:45 2026 GMT
  host: marianaoncology.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mariana Oncology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mariana Oncology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mariana Oncology
provider_slug: mariana-oncology
slug: mariana-oncology-domain-security
source_filename: mariana-oncology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marianaoncology.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 01:13:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: marianaoncology.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mariana-oncology/refs/heads/main/security/mariana-oncology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Radiopharmaceuticals
- Radioligand Therapy
- Life Sciences
- Healthcare
- Clinical Research
---
