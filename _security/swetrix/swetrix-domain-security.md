---
api_specs:
- filename: swetrix-events-api-openapi.yml
  format: yaml
  label: Swetrix Events API
  slug: swetrix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-events-api-openapi.yml
- filename: swetrix-annotations-api-openapi.yml
  format: yaml
  label: Swetrix Annotations API
  slug: swetrix-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-annotations-api-openapi.yml
- filename: swetrix-custom-events-api-openapi.yml
  format: yaml
  label: Swetrix Custom Events API
  slug: swetrix-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-custom-events-api-openapi.yml
- filename: swetrix-errors-api-openapi.yml
  format: yaml
  label: Swetrix Errors API
  slug: swetrix-errors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-errors-api-openapi.yml
- filename: swetrix-feature-flags-api-openapi.yml
  format: yaml
  label: Swetrix Feature Flags API
  slug: swetrix-feature-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-feature-flags-api-openapi.yml
- filename: swetrix-funnels-api-openapi.yml
  format: yaml
  label: Swetrix Funnels API
  slug: swetrix-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-funnels-api-openapi.yml
- filename: swetrix-organisations-api-openapi.yml
  format: yaml
  label: Swetrix Organisations API
  slug: swetrix-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-organisations-api-openapi.yml
- filename: swetrix-performance-api-openapi.yml
  format: yaml
  label: Swetrix Performance API
  slug: swetrix-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-performance-api-openapi.yml
- filename: swetrix-projects-api-openapi.yml
  format: yaml
  label: Swetrix Projects API
  slug: swetrix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-projects-api-openapi.yml
- filename: swetrix-revenue-api-openapi.yml
  format: yaml
  label: Swetrix Revenue API
  slug: swetrix-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-revenue-api-openapi.yml
- filename: swetrix-sessions-api-openapi.yml
  format: yaml
  label: Swetrix Sessions API
  slug: swetrix-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-sessions-api-openapi.yml
- filename: swetrix-traffic-api-openapi.yml
  format: yaml
  label: Swetrix Traffic API
  slug: swetrix-traffic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-traffic-api-openapi.yml
- filename: swetrix-views-api-openapi.yml
  format: yaml
  label: Swetrix Views API
  slug: swetrix-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/openapi/swetrix-views-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: swetrix.com
  spf: true
hosts:
- cert_expires: Sep 17 23:14:33 2026 GMT
  host: swetrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 15 21:04:01 2026 GMT
  host: api.swetrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swetrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swetrix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Swetrix
provider_slug: swetrix
slug: swetrix-domain-security
source_filename: swetrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swetrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.swetrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 15 21:04:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: swetrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swetrix/refs/heads/main/security/swetrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Cookieless Tracking
- GDPR Compliant
- Open Source
- Privacy
- Real-Time Analytics
- Web Analytics
---
