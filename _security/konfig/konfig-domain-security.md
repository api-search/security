---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: konfigthis.com
  spf: true
hosts:
- cert_expires: Sep  8 08:31:18 2026 GMT
  host: konfigthis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Konfig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Konfig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Konfig
provider_slug: konfig
slug: konfig-domain-security
source_filename: konfig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konfigthis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 08:31:18 2026 GMT\n  hsts: false\ndomains:\n- domain: konfigthis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/konfig/refs/heads/main/security/konfig-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Documentation
- CLI
- Developer Tools
- OpenAPI
- Postman
- SDK Generation
- Sunset
---
