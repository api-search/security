---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fluxx.io
  spf: true
hosts:
- cert_expires: Sep 16 18:30:04 2026 GMT
  host: www.fluxx.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fluxx Grants Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluxx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fluxx
provider_slug: fluxx-grants
slug: fluxx-grants-domain-security
source_filename: fluxx-grants-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fluxx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:30:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluxx.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluxx-grants/refs/heads/main/security/fluxx-grants-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Grants Management
- Grantmaking
- Nonprofit
- Philanthropy
- Foundations
- REST API
---
