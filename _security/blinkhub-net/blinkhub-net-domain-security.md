---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blinkhub.net
  spf: true
hosts:
- cert_expires: Dec 17 17:05:33 2026 GMT
  host: blinkhub.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blinkhub Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlinkHub Korea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlinkHub Korea
provider_slug: blinkhub-net
slug: blinkhub-net-domain-security
source_filename: blinkhub-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkhub.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 17:05:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blinkhub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blinkhub-net/security/blinkhub-net-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Artificial Intelligence
- PressRelease
- Media Distribution
- SEO
- Automation
---
