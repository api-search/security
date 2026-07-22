---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fda.gov
  spf: true
hosts:
- cert_expires: Mar 13 16:54:46 2027 GMT
  host: www.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fda Regulations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FDA Regulations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FDA Regulations
provider_slug: fda-regulations
slug: fda-regulations-domain-security
source_filename: fda-regulations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 16:54:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/security/fda-regulations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Food Safety
- Healthcare
- Medical Devices
- Pharmaceuticals
- Regulatory Compliance
---
