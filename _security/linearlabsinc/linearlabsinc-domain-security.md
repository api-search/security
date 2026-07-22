---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: linearlabsinc.com
  spf: true
hosts:
- cert_expires: Oct 14 09:05:17 2026 GMT
  host: linearlabsinc.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linearlabsinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linear Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Linear Labs
provider_slug: linearlabsinc
slug: linearlabsinc-domain-security
source_filename: linearlabsinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linearlabsinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:05:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linearlabsinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linearlabsinc/refs/heads/main/security/linearlabsinc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electric Motors
- Industrial
- Hardware
- Manufacturing
- Energy
- Wind Energy
- Defense
- Nuclear
- Mining
---
