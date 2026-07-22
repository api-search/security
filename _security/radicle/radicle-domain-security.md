---
api_specs:
- filename: radicle-httpd-openapi.yml
  format: yaml
  label: Radicle HTTP API
  slug: radicle-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radicle/refs/heads/main/openapi/radicle-httpd-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: radicle.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: radicle.network
  spf: true
hosts:
- cert_expires: Sep 28 15:44:54 2026 GMT
  host: radicle.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 21:39:52 2026 GMT
  host: radicle.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 12:13:19 2026 GMT
  host: seed.radicle.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Radicle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Radicle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Radicle
provider_slug: radicle
slug: radicle-domain-security
source_filename: radicle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: radicle.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:44:54 2026 GMT\n  hsts: false\n- host: radicle.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:39:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: seed.radicle.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:13:19 2026 GMT\n  hsts: false\ndomains:\n- domain: radicle.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: radicle.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radicle/refs/heads/main/security/radicle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Code Collaboration
- Git
- Peer-to-Peer
- Version Control
- Open Source
- Decentralized
- Developer Tools API
---
