---
api_specs:
- filename: marqeta-core-api-openapi.yml
  format: yaml
  label: Marqeta Core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-core-api-openapi.yml
- filename: marqeta-diva-api-openapi.yml
  format: yaml
  label: Marqeta Diva API
  slug: diva-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/openapi/marqeta-diva-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marqeta.com
  spf: true
hosts:
- cert_expires: Sep 27 19:54:00 2026 GMT
  host: www.marqeta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: sandbox-api.marqeta.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: diva-api.marqeta.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Marqeta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marqeta, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marqeta
provider_slug: marqeta
slug: marqeta-domain-security
source_filename: marqeta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marqeta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:54:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox-api.marqeta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\n- host: diva-api.marqeta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: marqeta.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marqeta/refs/heads/main/security/marqeta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FinTech
- BaaS
- Card Issuing
- Payments
- Embedded Finance
---
