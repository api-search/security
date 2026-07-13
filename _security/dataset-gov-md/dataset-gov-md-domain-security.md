---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dataset.gov.md
  spf: false
hosts:
- cert_expires: Dec 20 05:07:49 2026 GMT
  host: dataset.gov.md
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dataset Gov Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dataset.gov.md (Portalul Datelor Deschise), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: dataset.gov.md (Portalul Datelor Deschise)
provider_slug: dataset-gov-md
slug: dataset-gov-md-domain-security
source_filename: dataset-gov-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataset.gov.md\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 05:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dataset.gov.md\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataset-gov-md/refs/heads/main/security/dataset-gov-md-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- National Government
- Moldova
- Europe
---
