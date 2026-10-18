---
api_specs:
- filename: aritma-accounts-api-openapi.yml
  format: yaml
  label: Aritma Accounts API
  slug: aritma-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-accounts-api-openapi.yml
- filename: aritma-aritma-api-api-openapi.yml
  format: yaml
  label: Aritma Aritma API
  slug: aritma-aritma-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-aritma-api-api-openapi.yml
- filename: aritma-banks-api-openapi.yml
  format: yaml
  label: Aritma Banks API
  slug: aritma-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-banks-api-openapi.yml
- filename: aritma-bulk-payments-api-openapi.yml
  format: yaml
  label: Aritma Bulk Payments API
  slug: aritma-bulk-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-bulk-payments-api-openapi.yml
- filename: aritma-companies-api-openapi.yml
  format: yaml
  label: Aritma Companies API
  slug: aritma-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-companies-api-openapi.yml
- filename: aritma-consents-api-openapi.yml
  format: yaml
  label: Aritma Consents API
  slug: aritma-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-consents-api-openapi.yml
- filename: aritma-events-api-openapi.yml
  format: yaml
  label: Aritma Events API
  slug: aritma-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-events-api-openapi.yml
- filename: aritma-mock-api-openapi.yml
  format: yaml
  label: Aritma Mock API
  slug: aritma-mock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/openapi/aritma-mock-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aritma.com
  spf: true
hosts:
- cert_expires: Jan  9 18:11:49 2027 GMT
  host: aritma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aritma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aritma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aritma
provider_slug: aritma
slug: aritma-domain-security
source_filename: aritma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aritma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:11:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aritma.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aritma/refs/heads/main/security/aritma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Finance
- Automation
- B2B
- Payments
---
