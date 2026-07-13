---
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zillow.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zillowgroup.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.zillow.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: www.zillowgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:59:59 2026 GMT
  host: bridgedataoutput.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zillow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zillow, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zillow
provider_slug: zillow
slug: zillow-domain-security
source_filename: zillow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zillow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.zillowgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: bridgedataoutput.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zillow.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zillowgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillow/refs/heads/main/security/zillow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bridge
- Brokers
- IDX
- Lenders
- Listings
- Mortgage
- MLS
- Real Estate
- Rentals
- RESO
---
