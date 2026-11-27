---
description: ''
domains:
- caa:
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: extrabold.tools
  spf: true
hosts:
- cert_expires: Dec 10 08:33:24 2026 GMT
  host: extrabold.tools
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Extrabold Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Extrabold Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Extrabold Tools
provider_slug: extrabold-tools
slug: extrabold-tools-domain-security
source_filename: extrabold-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: extrabold.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 08:33:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: extrabold.tools\n  dnssec: false\n  caa:\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/extrabold-tools/security/extrabold-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- 3D Printing
- Browser Tools
- Maker
- Gridfinity
---
