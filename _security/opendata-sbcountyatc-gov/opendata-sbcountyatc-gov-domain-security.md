---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sbcountyatc.gov
  spf: true
hosts:
- cert_expires: Aug 31 21:19:38 2026 GMT
  host: opendata.sbcountyatc.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Sbcountyatc Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for San Bernardino County ATC OpenData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: San Bernardino County ATC OpenData
provider_slug: opendata-sbcountyatc-gov
slug: opendata-sbcountyatc-gov-domain-security
source_filename: opendata-sbcountyatc-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.sbcountyatc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:19:38 2026 GMT\n  hsts: false\ndomains:\n- domain: sbcountyatc.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-sbcountyatc-gov/refs/heads/main/security/opendata-sbcountyatc-gov-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- County Government
- United States
---
