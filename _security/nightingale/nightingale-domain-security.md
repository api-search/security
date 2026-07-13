---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nightingale.rest
  spf: true
hosts:
- cert_expires: Sep 24 12:46:51 2026 GMT
  host: nightingale.rest
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nightingale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nightingale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nightingale
provider_slug: nightingale
slug: nightingale-domain-security
source_filename: nightingale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nightingale.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:46:51 2026 GMT\n  hsts: false\ndomains:\n- domain: nightingale.rest\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nightingale/refs/heads/main/security/nightingale-domain-security.yml
summary_line: TLSv1.3
tags:
- Clients
- GUI
- REST Client
- Windows
---
