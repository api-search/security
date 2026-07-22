---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "amazon.com"
  - 0 iodef "mailto:cybersecurity@eqt.com"
  - 0 issue "cloudflare.com"
  - 0 issue "verisign.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: eqt.com
  spf: true
hosts:
- cert_expires: Sep 20 17:53:36 2026 GMT
  host: www.eqt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eqt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EQT Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EQT Corporation
provider_slug: eqt
slug: eqt-domain-security
source_filename: eqt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eqt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:53:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eqt.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"amazon.com\"\n  - 0 iodef \"mailto:cybersecurity@eqt.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"verisign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eqt/refs/heads/main/security/eqt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Natural Gas
- Oil and Gas
- Appalachian Basin
- Fortune 1000
---
