---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hivex.si
  spf: true
hosts:
- cert_expires: Dec 31 14:45:09 2026 GMT
  host: hivex.si
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hivex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hivex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hivex
provider_slug: hivex-si
slug: hivex-si-domain-security
source_filename: hivex-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hivex.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 14:45:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hivex.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hivex-si/security/hivex-si-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Domain
- Marketplace
- Artificial Intelligence
- Software
- Premium
---
