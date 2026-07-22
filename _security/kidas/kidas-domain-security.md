---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getkidas.com
  spf: true
hosts:
- cert_expires: Oct 15 06:12:42 2026 GMT
  host: getkidas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kidas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kidas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kidas
provider_slug: kidas
slug: kidas-domain-security
source_filename: kidas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkidas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 06:12:42 2026 GMT\n  hsts: false\ndomains:\n- domain: getkidas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kidas/refs/heads/main/security/kidas-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Trust and Safety
- Scam Detection
- Fraud Prevention
- Cybersecurity
- Gaming
- Deepfake Protection
- Discord
---
