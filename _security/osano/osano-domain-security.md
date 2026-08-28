---
api_specs:
- filename: osano-customer-rest-api-openapi.yml
  format: yaml
  label: Osano Customer REST API
  slug: osano-customer-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-customer-rest-api-openapi.yml
- filename: osano-unified-consent-core-api-openapi.yml
  format: yaml
  label: Osano Unified Consent Core API
  slug: osano-unified-consent-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/openapi/osano-unified-consent-core-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: osano.com
  spf: true
hosts:
- cert_expires: Nov 17 21:59:06 2026 GMT
  host: www.osano.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: developers.osano.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.osano.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osano, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Osano
provider_slug: osano
slug: osano-domain-security
source_filename: osano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 21:59:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.osano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.osano.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: osano.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osano/refs/heads/main/security/osano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data Privacy
- Consent Management
- Compliance
- GDPR
- CCPA
- Cookie Consent
- Subject Rights
- Data Mapping
- Vendor Risk
- Privacy Assessments
- Governance Risk Compliance
---
