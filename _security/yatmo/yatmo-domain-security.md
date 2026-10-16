---
api_specs:
- filename: yatmo-bikepaths-api-openapi.yml
  format: yaml
  label: Yatmo Bike Paths API
  slug: yatmo-bikepaths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-bikepaths-api-openapi.yml
- filename: yatmo-categories-api-openapi.yml
  format: yaml
  label: Yatmo Categories API
  slug: yatmo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-categories-api-openapi.yml
- filename: yatmo-enrichment-api-openapi.yml
  format: yaml
  label: Yatmo Enrichment API
  slug: yatmo-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-enrichment-api-openapi.yml
- filename: yatmo-frenchneighbourhoods-api-openapi.yml
  format: yaml
  label: Yatmo French Neighbourhoods API
  slug: yatmo-frenchneighbourhoods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-frenchneighbourhoods-api-openapi.yml
- filename: yatmo-geolocation-api-openapi.yml
  format: yaml
  label: Yatmo Geolocation API
  slug: yatmo-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geolocation-api-openapi.yml
- filename: yatmo-geopositionencoder-api-openapi.yml
  format: yaml
  label: Yatmo Geo Position Encoder API
  slug: yatmo-geopositionencoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geopositionencoder-api-openapi.yml
- filename: yatmo-image-api-openapi.yml
  format: yaml
  label: Yatmo Image API
  slug: yatmo-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-image-api-openapi.yml
- filename: yatmo-immotopcategories-api-openapi.yml
  format: yaml
  label: Yatmo Immotop Categories API
  slug: yatmo-immotopcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-immotopcategories-api-openapi.yml
- filename: yatmo-isochrone-api-openapi.yml
  format: yaml
  label: Yatmo Isochrone API
  slug: yatmo-isochrone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-isochrone-api-openapi.yml
- filename: yatmo-nearcheck-api-openapi.yml
  format: yaml
  label: Yatmo Near Check API
  slug: yatmo-nearcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-nearcheck-api-openapi.yml
- filename: yatmo-neighbourhood-api-openapi.yml
  format: yaml
  label: Yatmo Neighbourhood API
  slug: yatmo-neighbourhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-neighbourhood-api-openapi.yml
- filename: yatmo-points-api-openapi.yml
  format: yaml
  label: Yatmo Points API
  slug: yatmo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-points-api-openapi.yml
- filename: yatmo-route-api-openapi.yml
  format: yaml
  label: Yatmo Route API
  slug: yatmo-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-route-api-openapi.yml
- filename: yatmo-scores-api-openapi.yml
  format: yaml
  label: Yatmo Scores API
  slug: yatmo-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-scores-api-openapi.yml
- filename: yatmo-shape-api-openapi.yml
  format: yaml
  label: Yatmo Shape API
  slug: yatmo-shape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-shape-api-openapi.yml
- filename: yatmo-simplifiedcategories-api-openapi.yml
  format: yaml
  label: Yatmo Simplified Categories API
  slug: yatmo-simplifiedcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-simplifiedcategories-api-openapi.yml
- filename: yatmo-summary-api-openapi.yml
  format: yaml
  label: Yatmo Summary API
  slug: yatmo-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-summary-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yatmo.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: yatmo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yatmo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yatmo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yatmo
provider_slug: yatmo
slug: yatmo-domain-security
source_filename: yatmo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yatmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yatmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/security/yatmo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- RealEstate
- LocationIntelligence
- MappingAPI
- POIData
---
