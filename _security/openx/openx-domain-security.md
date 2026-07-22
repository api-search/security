---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "digicert.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openx.com
  spf: true
hosts:
- cert_expires: Sep  1 23:03:47 2026 GMT
  host: www.openx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenX
provider_slug: openx
slug: openx-domain-security
source_filename: openx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:03:47 2026 GMT\n  hsts: false\ndomains:\n- domain: openx.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openx/refs/heads/main/security/openx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Programmatic Advertising
- Ad Exchange
- Supply Side Platform
- SSP
- Real Time Bidding
- OpenRTB
- Header Bidding
- Prebid
- AdTech
- CTV
- Video Advertising
- Display Advertising
- Curation
- Identity
---
