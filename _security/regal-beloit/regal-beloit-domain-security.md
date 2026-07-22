---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regalrexnord.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: regal-beloit.com
  spf: true
hosts:
- cert_expires: Sep 25 22:25:57 2026 GMT
  host: www.regalrexnord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.regal-beloit.com
  https: false
kind: domain-security
layout: security
method: probed
name: Regal Beloit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for regal-beloit, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: regal-beloit
provider_slug: regal-beloit
slug: regal-beloit-domain-security
source_filename: regal-beloit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regalrexnord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:25:57 2026 GMT\n  hsts: false\n- host: www.regal-beloit.com\n  https: false\ndomains:\n- domain: regalrexnord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: regal-beloit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-beloit/refs/heads/main/security/regal-beloit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electric Motors
- Power Transmission
- Industrial Manufacturing
- HVAC
- Motion Control
- Power Generation
- Fortune 1000
---
