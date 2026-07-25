---
api_specs:
- filename: looker-auth-api-openapi.yml
  format: yaml
  label: Looker Auth API
  slug: looker-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-auth-api-openapi.yml
- filename: looker-dashboard-api-openapi.yml
  format: yaml
  label: Looker Dashboard API
  slug: looker-dashboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-dashboard-api-openapi.yml
- filename: looker-look-api-openapi.yml
  format: yaml
  label: Looker Look API
  slug: looker-look-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-look-api-openapi.yml
- filename: looker-query-api-openapi.yml
  format: yaml
  label: Looker Query API
  slug: looker-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-query-api-openapi.yml
- filename: looker-user-api-openapi.yml
  format: yaml
  label: Looker User API
  slug: looker-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/openapi/looker-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: looker.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Aug 18 03:12:56 2026 GMT
  host: developers.looker.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: your-instance.looker.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 14 08:37:10 2026 GMT
  host: docs.cloud.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Looker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Looker, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Looker
provider_slug: looker
slug: looker-domain-security
source_filename: looker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.looker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 03:12:56 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: your-instance.looker.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\n- host: docs.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: looker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/security/looker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
---
