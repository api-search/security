---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tigrisdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: storage.dev
  spf: false
hosts:
- cert_expires: Sep 15 19:02:15 2026 GMT
  host: www.tigrisdata.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:20:01 2026 GMT
  host: t3.storage.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tigris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tigris, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tigris
provider_slug: tigris
slug: tigris-domain-security
source_filename: tigris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tigrisdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: t3.storage.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:20:01 2026 GMT\n  hsts: null\ndomains:\n- domain: tigrisdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: storage.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tigris/refs/heads/main/security/tigris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Object Storage
- Cloud Storage
- S3 Compatible
- Storage
- AI Infrastructure
- Agents
- Data Infrastructure
---
