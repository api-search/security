---
api_specs:
- filename: fermyon-accounts-api-openapi.yml
  format: yaml
  label: Fermyon accounts API
  slug: fermyon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-accounts-api-openapi.yml
- filename: fermyon-apps-api-openapi.yml
  format: yaml
  label: Fermyon apps API
  slug: fermyon-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-apps-api-openapi.yml
- filename: fermyon-auth-tokens-api-openapi.yml
  format: yaml
  label: Fermyon auth-tokens API
  slug: fermyon-auth-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-auth-tokens-api-openapi.yml
- filename: fermyon-channels-api-openapi.yml
  format: yaml
  label: Fermyon channels API
  slug: fermyon-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-channels-api-openapi.yml
- filename: fermyon-custom-domains-api-openapi.yml
  format: yaml
  label: Fermyon custom-domains API
  slug: fermyon-custom-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-custom-domains-api-openapi.yml
- filename: fermyon-device-codes-api-openapi.yml
  format: yaml
  label: Fermyon device-codes API
  slug: fermyon-device-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-device-codes-api-openapi.yml
- filename: fermyon-key-value-pairs-api-openapi.yml
  format: yaml
  label: Fermyon key-value-pairs API
  slug: fermyon-key-value-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-pairs-api-openapi.yml
- filename: fermyon-key-value-stores-api-openapi.yml
  format: yaml
  label: Fermyon key-value-stores API
  slug: fermyon-key-value-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-key-value-stores-api-openapi.yml
- filename: fermyon-oci-api-openapi.yml
  format: yaml
  label: Fermyon oci API
  slug: fermyon-oci-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-oci-api-openapi.yml
- filename: fermyon-payments-api-openapi.yml
  format: yaml
  label: Fermyon payments API
  slug: fermyon-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-payments-api-openapi.yml
- filename: fermyon-personal-access-tokens-api-openapi.yml
  format: yaml
  label: Fermyon personal-access-tokens API
  slug: fermyon-personal-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-personal-access-tokens-api-openapi.yml
- filename: fermyon-revisions-api-openapi.yml
  format: yaml
  label: Fermyon revisions API
  slug: fermyon-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-revisions-api-openapi.yml
- filename: fermyon-sql-databases-api-openapi.yml
  format: yaml
  label: Fermyon sql-databases API
  slug: fermyon-sql-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-sql-databases-api-openapi.yml
- filename: fermyon-variable-pairs-api-openapi.yml
  format: yaml
  label: Fermyon variable-pairs API
  slug: fermyon-variable-pairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/openapi/fermyon-variable-pairs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fermyon.com
  spf: true
hosts:
- cert_expires: Sep 10 20:42:46 2026 GMT
  host: developer.fermyon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 19:11:40 2026 GMT
  host: www.fermyon.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:52:52 2026 GMT
  host: cloud.fermyon.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fermyon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fermyon, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fermyon
provider_slug: fermyon
slug: fermyon-domain-security
source_filename: fermyon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:42:46 2026 GMT\n  hsts: false\n- host: www.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:11:40 2026 GMT\n  hsts: null\n- host: cloud.fermyon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:52:52 2026 GMT\n  hsts: false\ndomains:\n- domain: fermyon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermyon/refs/heads/main/security/fermyon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Compute
- Functions
- WebAssembly
- Serverless
---
