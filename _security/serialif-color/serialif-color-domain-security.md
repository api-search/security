---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: serialif.com
  spf: true
hosts:
- cert_expires: Oct  4 06:55:44 2026 GMT
  host: color.serialif.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serialif Color Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serialif Color, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Serialif Color
provider_slug: serialif-color
slug: serialif-color-domain-security
source_filename: serialif-color-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: color.serialif.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 06:55:44 2026 GMT\n  hsts: false\ndomains:\n- domain: serialif.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serialif-color/refs/heads/main/security/serialif-color-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---
