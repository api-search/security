---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reapit.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: reapit.cloud
  spf: true
hosts:
- cert_expires: Oct 15 03:20:54 2026 GMT
  host: www.reapit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 00:22:55 2026 GMT
  host: foundations-documentation.reapit.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: platform.reapit.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reapit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reapit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Reapit
provider_slug: reapit
slug: reapit-domain-security
source_filename: reapit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reapit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: foundations-documentation.reapit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 00:22:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.reapit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: reapit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: reapit.cloud\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reapit/refs/heads/main/security/reapit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- United Kingdom
- PropTech
- CRM
- Estate Agents
- Property Listings
- Property Management
- Rentals
- Conveyancing
- Australia
---
