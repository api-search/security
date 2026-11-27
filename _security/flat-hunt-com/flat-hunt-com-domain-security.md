---
description: ''
domains:
- caa:
  - dcl1e3sz.up.railway.app.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: flat-hunt.com
  spf: false
hosts:
- cert_expires: Dec 17 15:35:14 2026 GMT
  host: flat-hunt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FlatHunt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FlatHunt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: FlatHunt
provider_slug: flat-hunt-com
slug: flat-hunt-com-domain-security
source_filename: flat-hunt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flat-hunt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 15:35:14 2026 GMT\n  hsts: false\ndomains:\n- domain: flat-hunt.com\n  dnssec: true\n  caa:\n  - dcl1e3sz.up.railway.app.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/flat-hunt-com/security/flat-hunt-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Real Estate
- Housing
- Berlin
- Expats
- Apartments
---
