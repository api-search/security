---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alternativeto.net
  spf: true
hosts:
- cert_expires: Sep 20 15:14:40 2026 GMT
  host: alternativeto.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alternativeto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlternativeTo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AlternativeTo
provider_slug: alternativeto
slug: alternativeto-domain-security
source_filename: alternativeto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alternativeto.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:14:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alternativeto.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alternativeto/refs/heads/main/security/alternativeto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Alternatives
- Reviews
- Software Discovery
- Software Directory
---
