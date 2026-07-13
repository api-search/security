---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: opendoor.com
  spf: true
hosts:
- cert_expires: Oct  2 18:10:52 2026 GMT
  host: www.opendoor.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opendoor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Opendoor
provider_slug: opendoor
slug: opendoor-domain-security
source_filename: opendoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendoor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:10:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: opendoor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendoor/refs/heads/main/security/opendoor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- Cash Offer
- Exclusives
- Homes
- iBuyer
- Listings
- Partners
- Real Estate
---
