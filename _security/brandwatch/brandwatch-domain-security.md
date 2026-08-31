---
api_specs:
- filename: brandwatch-client-api-openapi.yml
  format: yaml
  label: Brandwatch Client API
  slug: brandwatch-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-client-api-openapi.yml
- filename: brandwatch-data-api-openapi.yml
  format: yaml
  label: Brandwatch Data API
  slug: brandwatch-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-data-api-openapi.yml
- filename: brandwatch-me-api-openapi.yml
  format: yaml
  label: Brandwatch Me API
  slug: brandwatch-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-me-api-openapi.yml
- filename: brandwatch-oauth-api-openapi.yml
  format: yaml
  label: Brandwatch OAUTH API
  slug: brandwatch-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-oauth-api-openapi.yml
- filename: brandwatch-project-api-openapi.yml
  format: yaml
  label: Brandwatch Project API
  slug: brandwatch-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-project-api-openapi.yml
- filename: brandwatch-projects-api-openapi.yml
  format: yaml
  label: Brandwatch Projects API
  slug: brandwatch-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-projects-api-openapi.yml
- filename: brandwatch-user-api-openapi.yml
  format: yaml
  label: Brandwatch User API
  slug: brandwatch-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/openapi/brandwatch-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandwatch.com
  spf: true
hosts:
- cert_expires: Oct 11 08:00:55 2026 GMT
  host: www.brandwatch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 06:57:42 2026 GMT
  host: api.brandwatch.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandwatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandwatch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandwatch
provider_slug: brandwatch
slug: brandwatch-domain-security
source_filename: brandwatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 08:00:55 2026 GMT\n  hsts: false\n- host: api.brandwatch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 06:57:42 2026 GMT\n  hsts: null\ndomains:\n- domain: brandwatch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandwatch/refs/heads/main/security/brandwatch-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Social-Media
- Social Media Monitoring
- Consumer Intelligence
- Brand Management
- Sentiment Analysis
---
