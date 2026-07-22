---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: virgosvs.com
  spf: true
hosts:
- cert_expires: Sep 21 10:04:51 2026 GMT
  host: virgosvs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virgo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Virgo
provider_slug: virgo
slug: virgo-domain-security
source_filename: virgo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virgosvs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 10:04:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virgosvs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgo/refs/heads/main/security/virgo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Healthcare
- Life Sciences
- Endoscopy
- Gastroenterology
- Clinical Trials
- Medical Imaging
- Foundation Models
---
