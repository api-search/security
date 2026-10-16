---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: seccl.tech
  spf: true
hosts:
- cert_expires: Dec 10 03:53:54 2026 GMT
  host: seccl.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seccl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seccl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seccl
provider_slug: seccl
slug: seccl-domain-security
source_filename: seccl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seccl.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:53:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: seccl.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seccl/refs/heads/main/security/seccl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Investment Platform
- Embedded Banking
- API
- B2B
---
