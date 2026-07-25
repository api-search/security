---
api_specs:
- filename: microsoft-bing-autosuggest-api-openapi.yml
  format: yaml
  label: Microsoft Bing Autosuggest API
  slug: microsoft-bing-autosuggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-autosuggest-api-openapi.yml
- filename: microsoft-bing-customsearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing CustomSearch API
  slug: microsoft-bing-customsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-customsearch-api-openapi.yml
- filename: microsoft-bing-entitysearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing EntitySearch API
  slug: microsoft-bing-entitysearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-entitysearch-api-openapi.yml
- filename: microsoft-bing-imagesearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing ImageSearch API
  slug: microsoft-bing-imagesearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-imagesearch-api-openapi.yml
- filename: microsoft-bing-newssearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing NewsSearch API
  slug: microsoft-bing-newssearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-newssearch-api-openapi.yml
- filename: microsoft-bing-spellcheck-api-openapi.yml
  format: yaml
  label: Microsoft Bing SpellCheck API
  slug: microsoft-bing-spellcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-spellcheck-api-openapi.yml
- filename: microsoft-bing-videosearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing VideoSearch API
  slug: microsoft-bing-videosearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-videosearch-api-openapi.yml
- filename: microsoft-bing-visualsearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing VisualSearch API
  slug: microsoft-bing-visualsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-visualsearch-api-openapi.yml
- filename: microsoft-bing-websearch-api-openapi.yml
  format: yaml
  label: Microsoft Bing WebSearch API
  slug: microsoft-bing-websearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/openapi/microsoft-bing-websearch-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan  5 19:53:18 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 22:43:39 2026 GMT
  host: api.bing.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Bing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Bing, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Bing
provider_slug: microsoft-bing
slug: microsoft-bing-domain-security
source_filename: microsoft-bing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bing.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 22:43:39 2026 GMT\n  hsts: null\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bing/refs/heads/main/security/microsoft-bing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Search
- Web Search
- Images
- Videos
- News
- Azure AI
- Autosuggest
- Visual Search
---
