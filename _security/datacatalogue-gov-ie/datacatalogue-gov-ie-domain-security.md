---
description: ''
domains:
- caa:
  - d2gt118tp88e7c.cloudfront.net.
  dmarc: false
  dnssec: true
  domain: datacatalogue.gov.ie
  spf: false
hosts:
- cert_expires: Sep 16 23:59:59 2026 GMT
  host: datacatalogue.gov.ie
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datacatalogue Gov Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ireland Open Data Catalogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Ireland Open Data Catalogue
provider_slug: datacatalogue-gov-ie
slug: datacatalogue-gov-ie-domain-security
source_filename: datacatalogue-gov-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datacatalogue.gov.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: datacatalogue.gov.ie\n  dnssec: true\n  caa:\n  - d2gt118tp88e7c.cloudfront.net.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacatalogue-gov-ie/refs/heads/main/security/datacatalogue-gov-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Ireland
---
