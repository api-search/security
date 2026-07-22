---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mavrx.co
  spf: true
hosts:
- cert_expires: Oct  7 02:06:09 2026 GMT
  host: mavrx.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mavrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mavrx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mavrx
provider_slug: mavrx
slug: mavrx-domain-security
source_filename: mavrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mavrx.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:06:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mavrx.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mavrx/refs/heads/main/security/mavrx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
