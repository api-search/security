---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beazer.com
  spf: true
hosts:
- cert_expires: Sep  2 23:59:59 2026 GMT
  host: www.beazer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beazer Homes Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beazer Homes USA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beazer Homes USA
provider_slug: beazer-homes-usa
slug: beazer-homes-usa-domain-security
source_filename: beazer-homes-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beazer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: beazer.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beazer-homes-usa/refs/heads/main/security/beazer-homes-usa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Homebuilder
- Real Estate
- Construction
- Residential
- Energy Efficiency
- Housing
- Consumer
- Fortune 1000
- NYSE
---
