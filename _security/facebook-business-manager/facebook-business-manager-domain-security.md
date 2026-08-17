---
api_specs:
- filename: facebook-business-manager-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Accounts API
  slug: facebook-business-manager-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-accounts-api-openapi.yml
- filename: facebook-business-manager-ad-creatives-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Creatives API
  slug: facebook-business-manager-ad-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-creatives-api-openapi.yml
- filename: facebook-business-manager-ad-images-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Images API
  slug: facebook-business-manager-ad-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-images-api-openapi.yml
- filename: facebook-business-manager-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Sets API
  slug: facebook-business-manager-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-sets-api-openapi.yml
- filename: facebook-business-manager-ads-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ads API
  slug: facebook-business-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ads-api-openapi.yml
- filename: facebook-business-manager-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Campaigns API
  slug: facebook-business-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-campaigns-api-openapi.yml
- filename: facebook-business-manager-comments-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Comments API
  slug: facebook-business-manager-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-comments-api-openapi.yml
- filename: facebook-business-manager-custom-audiences-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Custom Audiences API
  slug: facebook-business-manager-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-custom-audiences-api-openapi.yml
- filename: facebook-business-manager-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Insights API
  slug: facebook-business-manager-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-insights-api-openapi.yml
- filename: facebook-business-manager-page-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Page Insights API
  slug: facebook-business-manager-page-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-page-insights-api-openapi.yml
- filename: facebook-business-manager-pages-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Pages API
  slug: facebook-business-manager-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-pages-api-openapi.yml
- filename: facebook-business-manager-photos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Photos API
  slug: facebook-business-manager-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-photos-api-openapi.yml
- filename: facebook-business-manager-posts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Posts API
  slug: facebook-business-manager-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-posts-api-openapi.yml
- filename: facebook-business-manager-videos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Videos API
  slug: facebook-business-manager-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-videos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meta.com
  spf: true
- caa:
  - 0 issue "digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af"
  dmarc: false
  dnssec: false
  domain: threads.net
  spf: true
hosts:
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: www.meta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:59:59 2026 GMT
  host: graph.threads.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facebook Business Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facebook Business Manager, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
slug: facebook-business-manager-domain-security
source_filename: facebook-business-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meta.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.threads.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: meta.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: threads.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; account=271b0beda0771d006aa3a6c11b05187d456d6c239b46cb5241196095b09c92af\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/security/facebook-business-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social Media
- Messaging
- Commerce
- Agents
- MCP
- Webhooks
---
