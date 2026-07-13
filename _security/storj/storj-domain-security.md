---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storj.io
  spf: true
hosts:
- cert_expires: Sep  9 20:04:29 2026 GMT
  host: docs.storj.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storj Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storj, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Storj
provider_slug: storj
slug: storj-domain-security
source_filename: storj-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.storj.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 20:04:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: storj.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storj/refs/heads/main/security/storj-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Storage And File Sharing
- Public APIs
---
