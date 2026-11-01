---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blinkco.io
  spf: true
hosts:
- cert_expires: Dec 26 00:56:51 2026 GMT
  host: blinkco.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blinkco Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blink
provider_slug: blinkco-io
slug: blinkco-io-domain-security
source_filename: blinkco-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkco.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:56:51 2026 GMT\n  hsts: false\ndomains:\n- domain: blinkco.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blinkco-io/security/blinkco-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- IoT
- Security
- Smart-Home
- Cloud
---
