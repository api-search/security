---
api_specs:
- filename: pirsch-access-links-api-openapi.yml
  format: yaml
  label: Pirsch Access Links API
  slug: pirsch-access-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-access-links-api-openapi.yml
- filename: pirsch-authentication-api-openapi.yml
  format: yaml
  label: Pirsch Authentication API
  slug: pirsch-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-authentication-api-openapi.yml
- filename: pirsch-clients-api-openapi.yml
  format: yaml
  label: Pirsch Clients API
  slug: pirsch-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-clients-api-openapi.yml
- filename: pirsch-conversion-goals-api-openapi.yml
  format: yaml
  label: Pirsch Conversion Goals API
  slug: pirsch-conversion-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-conversion-goals-api-openapi.yml
- filename: pirsch-domains-api-openapi.yml
  format: yaml
  label: Pirsch Domains API
  slug: pirsch-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-domains-api-openapi.yml
- filename: pirsch-email-reports-api-openapi.yml
  format: yaml
  label: Pirsch Email Reports API
  slug: pirsch-email-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-email-reports-api-openapi.yml
- filename: pirsch-funnels-api-openapi.yml
  format: yaml
  label: Pirsch Funnels API
  slug: pirsch-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-funnels-api-openapi.yml
- filename: pirsch-members-api-openapi.yml
  format: yaml
  label: Pirsch Members API
  slug: pirsch-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-members-api-openapi.yml
- filename: pirsch-short-links-api-openapi.yml
  format: yaml
  label: Pirsch Short Links API
  slug: pirsch-short-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-short-links-api-openapi.yml
- filename: pirsch-statistics-api-openapi.yml
  format: yaml
  label: Pirsch Statistics API
  slug: pirsch-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-statistics-api-openapi.yml
- filename: pirsch-tracking-api-openapi.yml
  format: yaml
  label: Pirsch Tracking API
  slug: pirsch-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-tracking-api-openapi.yml
- filename: pirsch-traffic-management-api-openapi.yml
  format: yaml
  label: Pirsch Traffic Management API
  slug: pirsch-traffic-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-traffic-management-api-openapi.yml
- filename: pirsch-user-api-openapi.yml
  format: yaml
  label: Pirsch User API
  slug: pirsch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-user-api-openapi.yml
- filename: pirsch-views-api-openapi.yml
  format: yaml
  label: Pirsch Views API
  slug: pirsch-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-views-api-openapi.yml
- filename: pirsch-webhooks-api-openapi.yml
  format: yaml
  label: Pirsch Webhooks API
  slug: pirsch-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/openapi/pirsch-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pirsch.io
  spf: true
hosts:
- cert_expires: Sep 21 21:22:28 2026 GMT
  host: pirsch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 02:52:28 2026 GMT
  host: docs.pirsch.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 03:11:56 2026 GMT
  host: api.pirsch.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pirsch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pirsch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pirsch
provider_slug: pirsch
slug: pirsch-domain-security
source_filename: pirsch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:22:28 2026 GMT\n  hsts: false\n- host: docs.pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:52:28 2026 GMT\n  hsts: false\n- host: api.pirsch.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:11:56 2026 GMT\n  hsts: null\ndomains:\n- domain: pirsch.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pirsch/refs/heads/main/security/pirsch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Web Analytics
- Privacy
- GDPR
- Cookie-Free
- Page Views
- Sessions
- Event
- Conversion Goals
- Funnels
- Traffic Sources
---
