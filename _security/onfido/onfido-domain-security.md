---
api_specs:
- filename: onfido-addresses-api-openapi.yml
  format: yaml
  label: Onfido Addresses API
  slug: onfido-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-addresses-api-openapi.yml
- filename: onfido-applicants-api-openapi.yml
  format: yaml
  label: Onfido Applicants API
  slug: onfido-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-applicants-api-openapi.yml
- filename: onfido-checks-api-openapi.yml
  format: yaml
  label: Onfido Checks API
  slug: onfido-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-checks-api-openapi.yml
- filename: onfido-documents-api-openapi.yml
  format: yaml
  label: Onfido Documents API
  slug: onfido-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-documents-api-openapi.yml
- filename: onfido-electronic-api-openapi.yml
  format: yaml
  label: Onfido Electronic API
  slug: onfido-electronic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-electronic-api-openapi.yml
- filename: onfido-extractions-api-openapi.yml
  format: yaml
  label: Onfido Extractions API
  slug: onfido-extractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-extractions-api-openapi.yml
- filename: onfido-live-api-openapi.yml
  format: yaml
  label: Onfido Live API
  slug: onfido-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-live-api-openapi.yml
- filename: onfido-motion-api-openapi.yml
  format: yaml
  label: Onfido Motion API
  slug: onfido-motion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-motion-api-openapi.yml
- filename: onfido-photos-api-openapi.yml
  format: yaml
  label: Onfido Photos API
  slug: onfido-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-photos-api-openapi.yml
- filename: onfido-pings-api-openapi.yml
  format: yaml
  label: Onfido Pings API
  slug: onfido-pings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-pings-api-openapi.yml
- filename: onfido-repeat-api-openapi.yml
  format: yaml
  label: Onfido Repeat API
  slug: onfido-repeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-repeat-api-openapi.yml
- filename: onfido-reports-api-openapi.yml
  format: yaml
  label: Onfido Reports API
  slug: onfido-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-reports-api-openapi.yml
- filename: onfido-results-api-openapi.yml
  format: yaml
  label: Onfido Results API
  slug: onfido-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-results-api-openapi.yml
- filename: onfido-token-api-openapi.yml
  format: yaml
  label: Onfido Token API
  slug: onfido-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-token-api-openapi.yml
- filename: onfido-watchlist-api-openapi.yml
  format: yaml
  label: Onfido Watchlist API
  slug: onfido-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-watchlist-api-openapi.yml
- filename: onfido-webhooks-api-openapi.yml
  format: yaml
  label: Onfido Webhooks API
  slug: onfido-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-webhooks-api-openapi.yml
- filename: onfido-workflows-api-openapi.yml
  format: yaml
  label: Onfido Workflows API
  slug: onfido-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/openapi/onfido-workflows-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "entrust.net"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: onfido.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: documentation.onfido.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onfido Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onfido, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Onfido
provider_slug: onfido
slug: onfido-domain-security
source_filename: onfido-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: documentation.onfido.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onfido.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onfido/refs/heads/main/security/onfido-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authentication
- Identity
- Verification
- Identity Verification
- KYC
- Document Verification
- Biometrics
---
