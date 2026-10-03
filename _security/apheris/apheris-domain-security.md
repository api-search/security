---
api_specs:
- filename: apheris-apheris-api-api-openapi.yml
  format: yaml
  label: Apheris Apheris API
  slug: apheris-apheris-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-apheris-api-api-openapi.yml
- filename: apheris-health-api-openapi.yml
  format: yaml
  label: Apheris Health API
  slug: apheris-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-health-api-openapi.yml
- filename: apheris-predict-async-api-openapi.yml
  format: yaml
  label: Apheris Predict Async API
  slug: apheris-predict-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-predict-async-api-openapi.yml
- filename: apheris-results-api-openapi.yml
  format: yaml
  label: Apheris Results API
  slug: apheris-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-results-api-openapi.yml
- filename: apheris-schema-api-openapi.yml
  format: yaml
  label: Apheris Schema API
  slug: apheris-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-schema-api-openapi.yml
- filename: apheris-ticket-api-openapi.yml
  format: yaml
  label: Apheris Ticket API
  slug: apheris-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-ticket-api-openapi.yml
- filename: apheris-weights-api-openapi.yml
  format: yaml
  label: Apheris Weights API
  slug: apheris-weights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/openapi/apheris-weights-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hiive.com
  spf: true
hosts:
- cert_expires: Dec 14 14:19:32 2026 GMT
  host: www.hiive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apheris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apheris, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Apheris
provider_slug: apheris
slug: apheris-domain-security
source_filename: apheris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 14:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hiive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apheris/refs/heads/main/security/apheris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Drug Discovery
- Federated Learning
- Biotechnology
---
