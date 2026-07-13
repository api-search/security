---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: qld.gov.au
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: geoscience.data.qld.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geoscience Data Qld Gov Au Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Queensland Geoscience Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Queensland Geoscience Data
provider_slug: geoscience-data-qld-gov-au
slug: geoscience-data-qld-gov-au-domain-security
source_filename: geoscience-data-qld-gov-au-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geoscience.data.qld.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: qld.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoscience-data-qld-gov-au/refs/heads/main/security/geoscience-data-qld-gov-au-domain-security.yml
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
