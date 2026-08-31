---
api_specs:
- filename: skipton-building-society-atm-api-openapi.yml
  format: yaml
  label: Skipton Building Society ATM API
  slug: skipton-building-society-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-atm-api-openapi.yml
- filename: skipton-building-society-bca-api-openapi.yml
  format: yaml
  label: Skipton Building Society BCA API
  slug: skipton-building-society-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-bca-api-openapi.yml
- filename: skipton-building-society-branch-api-openapi.yml
  format: yaml
  label: Skipton Building Society Branch API
  slug: skipton-building-society-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-branch-api-openapi.yml
- filename: skipton-building-society-ccc-api-openapi.yml
  format: yaml
  label: Skipton Building Society CCC API
  slug: skipton-building-society-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-ccc-api-openapi.yml
- filename: skipton-building-society-pca-api-openapi.yml
  format: yaml
  label: Skipton Building Society PCA API
  slug: skipton-building-society-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-pca-api-openapi.yml
- filename: skipton-building-society-sme-api-openapi.yml
  format: yaml
  label: Skipton Building Society SME API
  slug: skipton-building-society-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/openapi/skipton-building-society-sme-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skipton.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.skipton.co.uk
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Skipton Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skipton Building Society, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skipton Building Society
provider_slug: skipton-building-society
slug: skipton-building-society-domain-security
source_filename: skipton-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skipton.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: skipton.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skipton-building-society/refs/heads/main/security/skipton-building-society-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Building Society
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Mortgages
- Savings
- Account Information
- Payments
---
