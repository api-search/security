---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: carta.healthcare
  spf: true
hosts:
- cert_expires: Oct 15 13:19:28 2026 GMT
  host: www.carta.healthcare
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carta Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carta Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Carta Healthcare
provider_slug: carta-healthcare
slug: carta-healthcare-domain-security
source_filename: carta-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carta.healthcare\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:19:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carta.healthcare\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carta-healthcare/refs/heads/main/security/carta-healthcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Health IT
- Clinical Data
- Artificial Intelligence
- Data Abstraction
- Clinical Registries
- Electronic Medical Records
- Analytics
- HIPAA
- Company
---
