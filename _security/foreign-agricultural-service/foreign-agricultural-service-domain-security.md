---
api_specs:
- filename: foreign-agricultural-service-fas-open-data-swagger.json
  format: json
  label: USDA FAS Open Data API
  slug: fas-open-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/_original/foreign-agricultural-service-fas-open-data-swagger.json
- filename: foreign-agricultural-service-esr-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service ESR API
  slug: foreign-agricultural-service-esr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-esr-api-openapi.yml
- filename: foreign-agricultural-service-gats-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service GATS API
  slug: foreign-agricultural-service-gats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-gats-api-openapi.yml
- filename: foreign-agricultural-service-psd-api-openapi.yml
  format: yaml
  label: Foreign Agricultural Service PSD API
  slug: foreign-agricultural-service-psd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/openapi/foreign-agricultural-service-psd-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 iodef "mailto:icam_as_notify@ocio.usda.gov"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: usda.gov
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: www.fas.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: apps.fas.usda.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Foreign Agricultural Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foreign Agricultural Service, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Foreign Agricultural Service
provider_slug: foreign-agricultural-service
slug: foreign-agricultural-service-domain-security
source_filename: foreign-agricultural-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fas.usda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: null\n- host: apps.fas.usda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usda.gov\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 iodef \"mailto:icam_as_notify@ocio.usda.gov\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nobserved_on_api_path:\n  note: >-\n    Added 2026-09-10 from a direct probe of the API itself. The automated prober records\n    hsts: null for apps.fas.usda.gov because it probes the host root, which returns a 500\n    ASP.NET error page with no HSTS header. The API path DOES set it: responses from\n    https://apps.fas.usda.gov/OpenData/api/esr/regions carry\n    `strict-transport-security:\
  \ max-age=31536000; includeSubdomains; preload` and\n    `x-content-type-options: nosniff`. Recorded here rather than by editing the machine-written\n    hosts[] block above, so the prober's own output stays honest about what it measured.\n  host: apps.fas.usda.gov\n  path: /OpenData/api/esr/regions\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  x_content_type_options: nosniff\n  fetched: '2026-09-10'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/foreign-agricultural-service/refs/heads/main/security/foreign-agricultural-service-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Agriculture
- Federal-Government
- Trade
- Open-Data
- Commodities
- Exports
- Government
---
