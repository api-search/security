---
api_specs:
- filename: looker-studio-assets-api-openapi.yml
  format: yaml
  label: Looker Studio Assets API
  slug: looker-studio-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-assets-api-openapi.yml
- filename: looker-studio-authentication-api-openapi.yml
  format: yaml
  label: Looker Studio Authentication API
  slug: looker-studio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-authentication-api-openapi.yml
- filename: looker-studio-configuration-api-openapi.yml
  format: yaml
  label: Looker Studio Configuration API
  slug: looker-studio-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-configuration-api-openapi.yml
- filename: looker-studio-data-api-openapi.yml
  format: yaml
  label: Looker Studio Data API
  slug: looker-studio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-data-api-openapi.yml
- filename: looker-studio-embed-api-openapi.yml
  format: yaml
  label: Looker Studio Embed API
  slug: looker-studio-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-embed-api-openapi.yml
- filename: looker-studio-manifest-api-openapi.yml
  format: yaml
  label: Looker Studio Manifest API
  slug: looker-studio-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-manifest-api-openapi.yml
- filename: looker-studio-oembed-api-openapi.yml
  format: yaml
  label: Looker Studio oEmbed API
  slug: looker-studio-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-oembed-api-openapi.yml
- filename: looker-studio-permissions-api-openapi.yml
  format: yaml
  label: Looker Studio Permissions API
  slug: looker-studio-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-permissions-api-openapi.yml
- filename: looker-studio-reports-api-openapi.yml
  format: yaml
  label: Looker Studio Reports API
  slug: looker-studio-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-reports-api-openapi.yml
- filename: looker-studio-schema-api-openapi.yml
  format: yaml
  label: Looker Studio Schema API
  slug: looker-studio-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-schema-api-openapi.yml
- filename: looker-studio-visualization-api-openapi.yml
  format: yaml
  label: Looker Studio Visualization API
  slug: looker-studio-visualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-visualization-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:37:10 2026 GMT
  host: console.cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: lookerstudio.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Looker Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Looker Studio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Looker Studio
provider_slug: looker-studio
slug: looker-studio-domain-security
source_filename: looker-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: console.cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lookerstudio.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/security/looker-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
---
