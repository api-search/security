---
api_specs:
- filename: crosbynews-com-air-api-openapi.yml
  format: yaml
  label: Crosby News Air API
  slug: crosbynews-com-air-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-air-api-openapi.yml
- filename: crosbynews-com-burn-ban-api-openapi.yml
  format: yaml
  label: Crosby News Burn Ban API
  slug: crosbynews-com-burn-ban-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-burn-ban-api-openapi.yml
- filename: crosbynews-com-calendar-api-openapi.yml
  format: yaml
  label: Crosby News Calendar API
  slug: crosbynews-com-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-calendar-api-openapi.yml
- filename: crosbynews-com-fishing-api-openapi.yml
  format: yaml
  label: Crosby News Fishing API
  slug: crosbynews-com-fishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-fishing-api-openapi.yml
- filename: crosbynews-com-health-api-openapi.yml
  format: yaml
  label: Crosby News Health API
  slug: crosbynews-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-health-api-openapi.yml
- filename: crosbynews-com-news-api-openapi.yml
  format: yaml
  label: Crosby News News API
  slug: crosbynews-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-news-api-openapi.yml
- filename: crosbynews-com-pollen-api-openapi.yml
  format: yaml
  label: Crosby News Pollen API
  slug: crosbynews-com-pollen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-pollen-api-openapi.yml
- filename: crosbynews-com-traffic-api-openapi.yml
  format: yaml
  label: Crosby News Traffic API
  slug: crosbynews-com-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-traffic-api-openapi.yml
- filename: crosbynews-com-tropics-api-openapi.yml
  format: yaml
  label: Crosby News Tropics API
  slug: crosbynews-com-tropics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-tropics-api-openapi.yml
- filename: crosbynews-com-water-api-openapi.yml
  format: yaml
  label: Crosby News Water API
  slug: crosbynews-com-water-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-water-api-openapi.yml
- filename: crosbynews-com-weather-api-openapi.yml
  format: yaml
  label: Crosby News Weather API
  slug: crosbynews-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosbynews-com/openapi/crosbynews-com-weather-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@crosbynews.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: crosbynews.com
  spf: true
hosts:
- cert_expires: Dec 24 20:27:55 2026 GMT
  host: crosbynews.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crosbynews Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crosby News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Crosby News
provider_slug: crosbynews-com
slug: crosbynews-com-domain-security
source_filename: crosbynews-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crosbynews.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 20:27:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crosbynews.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@crosbynews.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/crosbynews-com/security/crosbynews-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
