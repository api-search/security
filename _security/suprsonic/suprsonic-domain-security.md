---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: suprsonic.ai
  spf: true
hosts:
- cert_expires: Sep 18 06:25:34 2026 GMT
  host: suprsonic.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Suprsonic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Suprsonic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Suprsonic
provider_slug: suprsonic
slug: suprsonic-domain-security
source_filename: suprsonic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suprsonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 06:25:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: suprsonic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suprsonic/refs/heads/main/security/suprsonic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Public APIs
---
