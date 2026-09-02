---
api_specs:
- filename: nhost-authentication-api-openapi.yml
  format: yaml
  label: Nhost authentication API
  slug: nhost-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-authentication-api-openapi.yml
- filename: nhost-documentation-api-openapi.yml
  format: yaml
  label: Nhost documentation API
  slug: nhost-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-documentation-api-openapi.yml
- filename: nhost-excludeme-api-openapi.yml
  format: yaml
  label: Nhost excludeme API
  slug: nhost-excludeme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-excludeme-api-openapi.yml
- filename: nhost-files-api-openapi.yml
  format: yaml
  label: Nhost files API
  slug: nhost-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-files-api-openapi.yml
- filename: nhost-operations-api-openapi.yml
  format: yaml
  label: Nhost operations API
  slug: nhost-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-operations-api-openapi.yml
- filename: nhost-security-api-openapi.yml
  format: yaml
  label: Nhost security API
  slug: nhost-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-security-api-openapi.yml
- filename: nhost-session-api-openapi.yml
  format: yaml
  label: Nhost session API
  slug: nhost-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-session-api-openapi.yml
- filename: nhost-storage-api-openapi.yml
  format: yaml
  label: Nhost storage API
  slug: nhost-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-storage-api-openapi.yml
- filename: nhost-system-api-openapi.yml
  format: yaml
  label: Nhost system API
  slug: nhost-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-system-api-openapi.yml
- filename: nhost-user-api-openapi.yml
  format: yaml
  label: Nhost user API
  slug: nhost-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-user-api-openapi.yml
- filename: nhost-verification-api-openapi.yml
  format: yaml
  label: Nhost verification API
  slug: nhost-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-verification-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhost.io
  spf: true
hosts:
- cert_expires: Aug 10 05:56:32 2026 GMT
  host: nhost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 12:38:19 2026 GMT
  host: docs.nhost.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nhost, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nhost
provider_slug: nhost
slug: nhost-domain-security
source_filename: nhost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nhost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 05:56:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.nhost.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:38:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nhost.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/security/nhost-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- GraphQL
- PostgreSQL
- Authentication
- File Storage
- Serverless Functions
- Real-Time
- Open-Source
- Firebase Alternative
- Backend-as-a-Service
---
