---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truevault.com
  spf: true
hosts:
- cert_expires: Aug 21 06:13:49 2026 GMT
  host: docs.truevault.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.truevault.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Truevault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueVault, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TrueVault
provider_slug: truevault
slug: truevault-domain-security
source_filename: truevault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.truevault.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 06:13:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.truevault.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: truevault.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truevault/refs/heads/main/security/truevault-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Privacy
- Security
- Compliance
- HIPAA
- Data Storage
- Encryption
- Identity
- Privacy
- PII
---
