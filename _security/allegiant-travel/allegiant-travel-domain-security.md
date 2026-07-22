---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: allegiantair.com
  spf: true
hosts:
- cert_expires: Sep 27 01:32:34 2026 GMT
  host: www.allegiantair.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 03:45:04 2026 GMT
  host: ir.allegiantair.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allegiant Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allegiant Travel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Allegiant Travel
provider_slug: allegiant-travel
slug: allegiant-travel-domain-security
source_filename: allegiant-travel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allegiantair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 01:32:34 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: ir.allegiantair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:45:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: allegiantair.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allegiant-travel/refs/heads/main/security/allegiant-travel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Airline
- Aviation
---
