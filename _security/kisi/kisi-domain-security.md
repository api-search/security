---
api_specs:
- filename: kisi-openapi-original.yml
  format: yaml
  label: Kisi API
  slug: kisi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/openapi/kisi-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getkisi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kisi.io
  spf: true
hosts:
- cert_expires: Sep 24 20:34:40 2026 GMT
  host: getkisi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:11:12 2026 GMT
  host: api.getkisi.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 20:11:12 2026 GMT
  host: api.kisi.io
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kisi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KISI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KISI
provider_slug: kisi
slug: kisi-domain-security
source_filename: kisi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkisi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:34:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getkisi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:11:12 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: api.kisi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:11:12 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: getkisi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kisi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kisi/refs/heads/main/security/kisi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical Access Control
- Security
- Identity
- IoT
- Building Management
- Access Control
- SaaS
---
