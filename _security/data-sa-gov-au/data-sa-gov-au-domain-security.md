---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sa.gov.au
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: data.sa.gov.au
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Sa Gov Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for data.sa.gov.au South Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: data.sa.gov.au South Australia
provider_slug: data-sa-gov-au
slug: data-sa-gov-au-domain-security
source_filename: data-sa-gov-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.sa.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sa.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-sa-gov-au/refs/heads/main/security/data-sa-gov-au-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Australia
---
