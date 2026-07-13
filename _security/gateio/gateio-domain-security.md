---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gate.io
  spf: true
hosts:
- cert_expires: Oct  4 01:13:54 2026 GMT
  host: www.gate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gateio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gateio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gateio
provider_slug: gateio
slug: gateio-domain-security
source_filename: gateio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:13:54 2026 GMT\n  hsts: null\ndomains:\n- domain: gate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gateio/refs/heads/main/security/gateio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cryptocurrency
- Public APIs
---
