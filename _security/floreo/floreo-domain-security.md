---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: floreovr.com
  spf: true
hosts:
- cert_expires: Aug 21 17:08:30 2026 GMT
  host: floreovr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Floreo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Floreo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Floreo
provider_slug: floreo
slug: floreo-domain-security
source_filename: floreo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: floreovr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 17:08:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: floreovr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/floreo/refs/heads/main/security/floreo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Virtual Reality
- Digital Therapeutics
- Behavioral Health
- Healthcare
- Autism
- Neurodiversity
- Telehealth
- Education
---
