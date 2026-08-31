---
api_specs:
- filename: leeds-building-society-atm-api-openapi.yml
  format: yaml
  label: Leeds Building Society ATM API
  slug: leeds-building-society-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-atm-api-openapi.yml
- filename: leeds-building-society-bca-api-openapi.yml
  format: yaml
  label: Leeds Building Society BCA API
  slug: leeds-building-society-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-bca-api-openapi.yml
- filename: leeds-building-society-branch-api-openapi.yml
  format: yaml
  label: Leeds Building Society Branch API
  slug: leeds-building-society-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-branch-api-openapi.yml
- filename: leeds-building-society-ccc-api-openapi.yml
  format: yaml
  label: Leeds Building Society CCC API
  slug: leeds-building-society-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-ccc-api-openapi.yml
- filename: leeds-building-society-pca-api-openapi.yml
  format: yaml
  label: Leeds Building Society PCA API
  slug: leeds-building-society-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-pca-api-openapi.yml
- filename: leeds-building-society-sme-api-openapi.yml
  format: yaml
  label: Leeds Building Society SME API
  slug: leeds-building-society-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/openapi/leeds-building-society-sme-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leedsbuildingsociety.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.leedsbuildingsociety.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Leeds Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leeds Building Society, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leeds Building Society
provider_slug: leeds-building-society
slug: leeds-building-society-domain-security
source_filename: leeds-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leedsbuildingsociety.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: leedsbuildingsociety.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leeds-building-society/refs/heads/main/security/leeds-building-society-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Building Society
- Mutual
- Savings
- Mortgages
- Open Banking
- PSD2
- OBIE
- United Kingdom
---
