---
api_specs:
- filename: sevalla-applications-api-openapi.yml
  format: yaml
  label: Sevalla Applications API
  slug: sevalla-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-applications-api-openapi.yml
- filename: sevalla-company-api-openapi.yml
  format: yaml
  label: Sevalla Company API
  slug: sevalla-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-company-api-openapi.yml
- filename: sevalla-databases-api-openapi.yml
  format: yaml
  label: Sevalla Databases API
  slug: sevalla-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-databases-api-openapi.yml
- filename: sevalla-deployments-api-openapi.yml
  format: yaml
  label: Sevalla Deployments API
  slug: sevalla-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-deployments-api-openapi.yml
- filename: sevalla-object-storage-api-openapi.yml
  format: yaml
  label: Sevalla Object Storage API
  slug: sevalla-object-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-object-storage-api-openapi.yml
- filename: sevalla-pipelines-api-openapi.yml
  format: yaml
  label: Sevalla Pipelines API
  slug: sevalla-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-pipelines-api-openapi.yml
- filename: sevalla-static-sites-api-openapi.yml
  format: yaml
  label: Sevalla Static Sites API
  slug: sevalla-static-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/openapi/sevalla-static-sites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sevalla.com
  spf: true
hosts:
- cert_expires: Oct  3 23:26:42 2026 GMT
  host: sevalla.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 05:43:40 2026 GMT
  host: api-docs.sevalla.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 22:43:33 2026 GMT
  host: api.sevalla.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sevalla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sevalla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sevalla
provider_slug: sevalla
slug: sevalla-domain-security
source_filename: sevalla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sevalla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:26:42 2026 GMT\n  hsts: false\n- host: api-docs.sevalla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:43:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sevalla.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:43:33 2026 GMT\n  hsts: null\ndomains:\n- domain: sevalla.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sevalla/refs/heads/main/security/sevalla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Hosting
- Platform-as-a-Service
- Cloud
- Deployment
- Databases
- Static Sites
- Object Storage
---
