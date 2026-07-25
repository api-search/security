---
api_specs:
- filename: smartnews-ad-api-openapi.yml
  format: yaml
  label: SmartNews ad API
  slug: smartnews-ad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-ad-api-openapi.yml
- filename: smartnews-ad-group-api-openapi.yml
  format: yaml
  label: SmartNews ad-group API
  slug: smartnews-ad-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-ad-group-api-openapi.yml
- filename: smartnews-article-category-api-openapi.yml
  format: yaml
  label: SmartNews article category API
  slug: smartnews-article-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-article-category-api-openapi.yml
- filename: smartnews-campaign-api-openapi.yml
  format: yaml
  label: SmartNews campaign API
  slug: smartnews-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-campaign-api-openapi.yml
- filename: smartnews-catalog-api-openapi.yml
  format: yaml
  label: SmartNews catalog API
  slug: smartnews-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-catalog-api-openapi.yml
- filename: smartnews-channel-alias-label-api-openapi.yml
  format: yaml
  label: SmartNews channel alias label API
  slug: smartnews-channel-alias-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-channel-alias-label-api-openapi.yml
- filename: smartnews-custom-audience-api-openapi.yml
  format: yaml
  label: SmartNews custom-audience API
  slug: smartnews-custom-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-custom-audience-api-openapi.yml
- filename: smartnews-developer-app-api-openapi.yml
  format: yaml
  label: SmartNews developer-app API
  slug: smartnews-developer-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-developer-app-api-openapi.yml
- filename: smartnews-insights-api-openapi.yml
  format: yaml
  label: SmartNews insights API
  slug: smartnews-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-insights-api-openapi.yml
- filename: smartnews-interests-api-openapi.yml
  format: yaml
  label: SmartNews interests API
  slug: smartnews-interests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-interests-api-openapi.yml
- filename: smartnews-locations-api-openapi.yml
  format: yaml
  label: SmartNews locations API
  slug: smartnews-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-locations-api-openapi.yml
- filename: smartnews-media-file-api-openapi.yml
  format: yaml
  label: SmartNews media-file API
  slug: smartnews-media-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-media-file-api-openapi.yml
- filename: smartnews-oauth-api-openapi.yml
  format: yaml
  label: SmartNews oauth API
  slug: smartnews-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-oauth-api-openapi.yml
- filename: smartnews-pixel-api-openapi.yml
  format: yaml
  label: SmartNews pixel API
  slug: smartnews-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-pixel-api-openapi.yml
- filename: smartnews-smart-view-article-keyword-api-openapi.yml
  format: yaml
  label: SmartNews smart view article keyword API
  slug: smartnews-smart-view-article-keyword-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-smart-view-article-keyword-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smartnews.com
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: www.smartnews.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: ads.smartnews.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartnews Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartNews, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SmartNews
provider_slug: smartnews
slug: smartnews-domain-security
source_filename: smartnews-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smartnews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ads.smartnews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smartnews.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/security/smartnews-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- News
- Advertising
- AdTech
- Marketing
- Media
- Campaign Management
---
