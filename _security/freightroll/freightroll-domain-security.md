---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: freightroll.com
  spf: true
hosts:
- cert_expires: Aug 21 11:43:53 2026 GMT
  host: freightroll.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freightroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreightRoll, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FreightRoll
provider_slug: freightroll
slug: freightroll-domain-security
source_filename: freightroll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freightroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 11:43:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: freightroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freightroll/refs/heads/main/security/freightroll-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Yard Management
- Supply Chain
- Freight
- Transportation
- Trucking
---
