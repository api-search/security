---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cotality.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issue "pki.goog"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corelogic.com
  spf: true
hosts:
- cert_expires: Oct  7 04:27:56 2026 GMT
  host: www.cotality.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: trestle-documentation.corelogic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 01:22:44 2026 GMT
  host: api.cotality.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trestle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trestle, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trestle
provider_slug: trestle
slug: trestle-domain-security
source_filename: trestle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cotality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:27:56 2026 GMT\n  hsts: false\n- host: trestle-documentation.corelogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: false\n- host: api.cotality.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 01:22:44 2026 GMT\n  hsts: null\ndomains:\n- domain: cotality.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: corelogic.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trestle/refs/heads/main/security/trestle-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Data Distribution
- OData
- RETS
- Listing Syndication
---
