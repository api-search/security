---
api_specs:
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-celebrity-api-openapi.yml
  format: yaml
  label: Fabric Origin Celebrity API
  slug: celebrity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-celebrity-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Video API
  slug: video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Image API
  slug: image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-common-metadata-api-openapi.yml
  format: yaml
  label: Fabric Origin Common Data API
  slug: common-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-common-metadata-api-openapi.yml
- filename: fabric-origin-entertainment-api-openapi.yml
  format: yaml
  label: Fabric Origin Entertainment API
  slug: fabric-origin-entertainment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-entertainment-api-openapi.yml
- filename: fabric-origin-images-api-openapi.yml
  format: yaml
  label: Fabric Origin Images API
  slug: fabric-origin-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-images-api-openapi.yml
- filename: fabric-origin-videos-api-openapi.yml
  format: yaml
  label: Fabric Origin Videos API
  slug: fabric-origin-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-videos-api-openapi.yml
- filename: fabric-origin-video-analytics-api-openapi.yml
  format: yaml
  label: Fabric Origin Video Analytics API
  slug: video-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-video-analytics-api-openapi.yml
- filename: fabric-origin-fandango-api-openapi.yml
  format: yaml
  label: Fabric Origin Fandango API
  slug: fandango-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-fandango-api-openapi.yml
- filename: fabric-origin-captions-translations-api-openapi.yml
  format: yaml
  label: Fabric Origin Captions and Translations API
  slug: captions-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-captions-translations-api-openapi.yml
- filename: fabric-origin-metacritic-api-openapi.yml
  format: yaml
  label: Fabric Origin Metacritic API
  slug: metacritic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-metacritic-api-openapi.yml
- filename: fabric-origin-common-sense-media-api-openapi.yml
  format: yaml
  label: Fabric Origin Common Sense Media API
  slug: common-sense-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-common-sense-media-api-openapi.yml
- filename: fabric-origin-rotten-tomatoes-api-openapi.yml
  format: yaml
  label: Fabric Origin Rotten Tomatoes API
  slug: rotten-tomatoes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rotten-tomatoes-api-openapi.yml
- filename: fabric-origin-rabbit-recommendations-api-openapi.yml
  format: yaml
  label: Fabric Origin Rabbit Recommendations API
  slug: rabbit-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-rabbit-recommendations-api-openapi.yml
- filename: fabric-origin-tv-grid-online-api-openapi.yml
  format: yaml
  label: Fabric Origin TV Grid Online API
  slug: tv-grid-online-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-tv-grid-online-api-openapi.yml
- filename: fabric-origin-katch-media-api-openapi.yml
  format: yaml
  label: Fabric Origin Katch Media API
  slug: katch-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/openapi/fabric-origin-katch-media-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabricdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: iva-api.com
  spf: false
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.fabricdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 17:40:01 2026 GMT
  host: knowledgebase.fabricdata.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: ee.iva-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Fabric Origin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fabric Origin, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fabric Origin
provider_slug: fabric-origin
slug: fabric-origin-domain-security
source_filename: fabric-origin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: knowledgebase.fabricdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 17:40:01 2026 GMT\n  hsts: null\n- host: ee.iva-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fabricdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: iva-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabric-origin/refs/heads/main/security/fabric-origin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Entertainment
- Metadata
- Movies
- Television
- Games
- Celebrities
- Trailers
- Images
- TV Listings
- Market Intelligence
- Media
- MCP
---
