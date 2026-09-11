---
api_specs:
- filename: first-american-financial-title-settlement-openapi.yml
  format: yaml
  label: First American Title & Settlement (Mortgage Services) API
  slug: first-american-financial-title-settlement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-title-settlement-openapi.yml
- filename: first-american-financial-property-openapi.yml
  format: yaml
  label: First American Property API
  slug: first-american-financial-property
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-property-openapi.yml
- filename: first-american-financial-ownership-openapi.yml
  format: yaml
  label: First American Ownership API
  slug: first-american-financial-ownership
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-ownership-openapi.yml
- filename: first-american-financial-occupancy-openapi.yml
  format: yaml
  label: First American Occupancy API
  slug: first-american-financial-occupancy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-occupancy-openapi.yml
- filename: first-american-financial-identity-openapi.yml
  format: yaml
  label: First American Identity API
  slug: first-american-financial-identity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-identity-openapi.yml
- filename: first-american-financial-bankruptcy-openapi.yml
  format: yaml
  label: First American Bankruptcy API
  slug: first-american-financial-bankruptcy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-bankruptcy-openapi.yml
- filename: first-american-financial-4506c-openapi.yml
  format: yaml
  label: First American 4506-C Tax Transcript API
  slug: first-american-financial-4506c
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-4506c-openapi.yml
- filename: first-american-financial-reverse-phone-openapi.yml
  format: yaml
  label: First American Reverse Phone Search API
  slug: first-american-financial-reverse-phone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-reverse-phone-openapi.yml
- filename: first-american-financial-reverse-address-openapi.yml
  format: yaml
  label: First American Reverse Address Search API
  slug: first-american-financial-reverse-address
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-reverse-address-openapi.yml
- filename: first-american-financial-scra-openapi.yml
  format: yaml
  label: First American Active Duty SCRA Search API
  slug: first-american-financial-scra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-scra-openapi.yml
- filename: first-american-financial-income-estimate-openapi.yml
  format: yaml
  label: First American Income Estimate API
  slug: first-american-financial-income-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-income-estimate-openapi.yml
- filename: first-american-financial-liens-judgments-fcra-openapi.yml
  format: yaml
  label: First American Liens & Judgments (FCRA) API
  slug: first-american-financial-liens-judgments-fcra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-liens-judgments-fcra-openapi.yml
- filename: first-american-financial-liens-judgments-non-fcra-openapi.yml
  format: yaml
  label: First American Liens & Judgments (Non-FCRA) API
  slug: first-american-financial-liens-judgments-non-fcra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-liens-judgments-non-fcra-openapi.yml
- filename: first-american-financial-watchlist-openapi.yml
  format: yaml
  label: First American Watchlist API
  slug: first-american-financial-watchlist
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-watchlist-openapi.yml
- filename: first-american-financial-nmls-openapi.yml
  format: yaml
  label: First American NMLS License Verification API
  slug: first-american-financial-nmls
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-nmls-openapi.yml
- filename: first-american-financial-clearsearch-openapi.yml
  format: yaml
  label: First American ClearSearch API
  slug: first-american-financial-clearsearch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/openapi/first-american-financial-clearsearch-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firstam.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "awstrust.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: firstam.io
  spf: true
hosts:
- cert_expires: Nov 17 19:38:28 2026 GMT
  host: www.firstam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:59:59 2026 GMT
  host: developer.firstam.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.firstam.io
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: First American Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First American Financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: First American Financial
provider_slug: first-american-financial
slug: first-american-financial-domain-security
source_filename: first-american-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 19:38:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.firstam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.firstam.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: firstam.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: firstam.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-american-financial/refs/heads/main/security/first-american-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Title Insurance
- Real-Estate
- Settlement Services
- Financial-Services
- Mortgage
- Property Data
- Identity Verification
- Regulatory Compliance
- Fortune 1000
---
