---
api_specs:
- filename: wellhub-com-integrations-openapi-original.json
  format: json
  label: Wellhub Integrations API
  slug: wellhub-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wellhub-com/refs/heads/main/openapi/wellhub-com-integrations-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellhub.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: wellhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: developer-hub.wellhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  3 23:59:59 2027 GMT
  host: api.clients.wellhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellhub Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wellhub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wellhub
provider_slug: wellhub-com
slug: wellhub-com-domain-security
source_filename: wellhub-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wellhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: developer-hub.wellhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\n- host: api.clients.wellhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: wellhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nx-evidence:\n  fetched: '2026-08-04'\n  observations:\n  - host: api.clients.wellhub.com\n    note: >-\n      The automated HEAD probe recorded hsts: null because the API gateway answers an unrouted / with\n      403 and no HSTS header. A live request to an actual route —\n      GET https://api.clients.wellhub.com/v1/companies (401) — DOES return\n      \"strict-transport-security: max-age=31536000;\
  \ includeSubDomains\", along with\n      \"x-content-type-options: nosniff\" and \"cache-control: no-store\". HSTS is enforced on the API\n      surface itself.\n  - domain: wellhub.com\n    note: >-\n      No CAA record and no DNSSEC. SPF and DMARC are both present, with DMARC policy p=reject.\n      Qualys SSL Labs grades the estate A+ per the trust center (security/wellhub-com-trust-center.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellhub-com/refs/heads/main/security/wellhub-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- corporate-wellness
- employee-benefits
- human-resources
- hr-tech
- eligibility
- workforce
- fitness
- wellbeing
- payroll
- sftp
- hris-integration
---
