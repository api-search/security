---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smartsign.com
  spf: true
hosts:
- cert_expires: Mar 24 21:43:35 2027 GMT
  host: smartsign.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartsign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartsign, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Smartsign
provider_slug: smartsign
slug: smartsign-domain-security
source_filename: smartsign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartsign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 21:43:35 2027 GMT\n  hsts: false\ndomains:\n- domain: smartsign.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartsign/refs/heads/main/security/smartsign-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Signage
- E-Commerce
- Labels
- Safety
- Compliance
- Retail
- Printing
---
