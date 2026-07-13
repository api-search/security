---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: banuba.com
  spf: true
hosts:
- cert_expires: Sep 14 23:25:57 2026 GMT
  host: www.banuba.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: docs.banuba.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Banuba Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Banuba, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Banuba
provider_slug: banuba
slug: banuba-domain-security
source_filename: banuba-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.banuba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:25:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.banuba.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: banuba.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banuba/refs/heads/main/security/banuba-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AR
- Augmented Reality
- Beauty
- Face Recognition
- Facial
- SDK
- Video
---
