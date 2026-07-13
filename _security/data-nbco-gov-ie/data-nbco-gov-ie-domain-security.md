---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nbco.gov.ie
  spf: true
hosts:
- cert_expires: Oct  3 01:43:58 2026 GMT
  host: data.nbco.gov.ie
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Nbco Gov Ie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NBCO Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NBCO Open Data
provider_slug: data-nbco-gov-ie
slug: data-nbco-gov-ie-domain-security
source_filename: data-nbco-gov-ie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.nbco.gov.ie\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:43:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nbco.gov.ie\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-nbco-gov-ie/refs/heads/main/security/data-nbco-gov-ie-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Ireland
---
