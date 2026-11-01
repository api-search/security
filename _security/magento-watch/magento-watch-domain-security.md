---
api_specs:
- filename: magento-watch-meta-api-openapi.yml
  format: yaml
  label: magento-watch Meta API
  slug: magento-watch-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-meta-api-openapi.yml
- filename: magento-watch-patches-api-openapi.yml
  format: yaml
  label: magento-watch Patches API
  slug: magento-watch-patches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-patches-api-openapi.yml
- filename: magento-watch-security-api-openapi.yml
  format: yaml
  label: magento-watch Security API
  slug: magento-watch-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-security-api-openapi.yml
- filename: magento-watch-upstream-fixes-api-openapi.yml
  format: yaml
  label: magento-watch Upstream Fixes API
  slug: magento-watch-upstream-fixes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-upstream-fixes-api-openapi.yml
- filename: magento-watch-versions-api-openapi.yml
  format: yaml
  label: magento-watch Versions API
  slug: magento-watch-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magento-watch/openapi/magento-watch-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: magento.watch
  spf: false
hosts:
- cert_expires: Jan 13 07:06:49 2027 GMT
  host: magento.watch
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Magento Watch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for magento-watch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: magento-watch
provider_slug: magento-watch
slug: magento-watch-domain-security
source_filename: magento-watch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magento.watch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 07:06:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: magento.watch\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/magento-watch/security/magento-watch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Magento
- API
- Lifecycle
- OpenSource
---
