---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: se-fi.com
  spf: true
hosts:
- cert_expires: Oct  5 03:50:29 2026 GMT
  host: www.se-fi.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stoneeagle F And I Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StoneEagle F&I, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StoneEagle F&I
provider_slug: stoneeagle-f-and-i
slug: stoneeagle-f-and-i-domain-security
source_filename: stoneeagle-f-and-i-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.se-fi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 03:50:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: se-fi.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stoneeagle-f-and-i/refs/heads/main/security/stoneeagle-f-and-i-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Finance and Insurance
- Dealership
- Automotive Retail
- DMS Integration
- Reporting
- Analytics
---
