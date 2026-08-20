---
api_specs:
- filename: neurable-core-api-openapi.yml
  format: yaml
  label: Neurable Core API
  slug: neurable-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-core-api-openapi.yml
- filename: neurable-oauth-api-openapi.yml
  format: yaml
  label: Neurable O Auth API
  slug: neurable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oauth-api-openapi.yml
- filename: neurable-oidc-api-openapi.yml
  format: yaml
  label: Neurable OIDC API
  slug: neurable-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-oidc-api-openapi.yml
- filename: neurable-open-api-openapi.yml
  format: yaml
  label: Neurable Open API
  slug: neurable-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-open-api-openapi.yml
- filename: neurable-protected-api-openapi.yml
  format: yaml
  label: Neurable Protected API
  slug: neurable-protected-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/openapi/neurable-protected-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neurable.com
  spf: true
hosts:
- cert_expires: Oct 15 04:18:24 2026 GMT
  host: www.neurable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 19:12:04 2026 GMT
  host: analytics-service.neurable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: pipe.neurable.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Neurable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neurable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neurable
provider_slug: neurable
slug: neurable-domain-security
source_filename: neurable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neurable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:18:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: analytics-service.neurable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:12:04 2026 GMT\n  hsts: null\n- host: pipe.neurable.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: neurable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurable/refs/heads/main/security/neurable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Neurotechnology
- Brain-Computer Interface
- EEG
- Neuroscience
- Wearables
- biosignals
- Hardware
- Consumer Electronics
- Research Tools
- cognitive-analytics
- Health Data
- Authentication
- OpenID Connect
---
