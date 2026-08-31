---
api_specs:
- filename: principality-building-society-atm-api-openapi.yml
  format: yaml
  label: Principality Building Society ATM API
  slug: principality-building-society-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-atm-api-openapi.yml
- filename: principality-building-society-bca-api-openapi.yml
  format: yaml
  label: Principality Building Society BCA API
  slug: principality-building-society-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-bca-api-openapi.yml
- filename: principality-building-society-branch-api-openapi.yml
  format: yaml
  label: Principality Building Society Branch API
  slug: principality-building-society-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-branch-api-openapi.yml
- filename: principality-building-society-ccc-api-openapi.yml
  format: yaml
  label: Principality Building Society CCC API
  slug: principality-building-society-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-ccc-api-openapi.yml
- filename: principality-building-society-pca-api-openapi.yml
  format: yaml
  label: Principality Building Society PCA API
  slug: principality-building-society-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-pca-api-openapi.yml
- filename: principality-building-society-sme-api-openapi.yml
  format: yaml
  label: Principality Building Society SME API
  slug: principality-building-society-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/openapi/principality-building-society-sme-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: principality.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.principality.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Principality Building Society Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Principality Building Society, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Principality Building Society
provider_slug: principality-building-society
slug: principality-building-society-domain-security
source_filename: principality-building-society-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.principality.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: principality.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/principality-building-society/refs/heads/main/security/principality-building-society-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Building Society
- Savings
- Mortgages
- Open Banking
- Open Data
- PSD2
- OBIE
- United Kingdom
- Wales
- Mutual
---
