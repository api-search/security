---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blinkcodes.com
  spf: true
hosts:
- cert_expires: Dec  7 11:32:09 2026 GMT
  host: blinkcodes.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blinkcodes Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlinkCodes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlinkCodes
provider_slug: blinkcodes-com
slug: blinkcodes-com-domain-security
source_filename: blinkcodes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blinkcodes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 11:32:09 2026 GMT\n  hsts: false\ndomains:\n- domain: blinkcodes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blinkcodes-com/security/blinkcodes-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Gift Cards
- eSIM
- Virtual Numbers
---
