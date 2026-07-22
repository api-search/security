---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild ";"
  - 0 issue "comodoca.com"
  dmarc: false
  dnssec: false
  domain: schaeffler.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.schaeffler.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Schaeffler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schaeffler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Schaeffler
provider_slug: schaeffler
slug: schaeffler-domain-security
source_filename: schaeffler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.schaeffler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: schaeffler.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schaeffler/refs/heads/main/security/schaeffler-domain-security.yml
summary_line: TLSv1.3
tags:
- Automotive
- Industrial
- Tier 1 Supplier
- Bearings
- Powertrain
- E-Mobility
---
