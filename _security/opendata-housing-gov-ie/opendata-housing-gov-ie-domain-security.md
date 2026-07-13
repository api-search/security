---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: housing.gov.ie
  spf: true
hosts:
- cert_expires: Sep 12 19:03:44 2026 GMT
  host: opendata.housing.gov.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Housing Gov Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Irish Housing Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Irish Housing Open Data
provider_slug: opendata-housing-gov-ie
slug: opendata-housing-gov-ie-domain-security
source_filename: opendata-housing-gov-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.housing.gov.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 19:03:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: housing.gov.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-housing-gov-ie/refs/heads/main/security/opendata-housing-gov-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Federal Government
- Ireland
---
