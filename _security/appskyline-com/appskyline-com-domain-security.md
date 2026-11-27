---
api_specs:
- filename: appskyline-com-apps-api-openapi.yml
  format: yaml
  label: AppSkyline Apps API
  slug: appskyline-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-apps-api-openapi.yml
- filename: appskyline-com-batch-api-openapi.yml
  format: yaml
  label: AppSkyline Batch API
  slug: appskyline-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-batch-api-openapi.yml
- filename: appskyline-com-google-play-publishing-api-openapi.yml
  format: yaml
  label: AppSkyline Google Play Publishing API
  slug: appskyline-com-google-play-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-google-play-publishing-api-openapi.yml
- filename: appskyline-com-keywords-api-openapi.yml
  format: yaml
  label: AppSkyline Keywords API
  slug: appskyline-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-keywords-api-openapi.yml
- filename: appskyline-com-metadata-api-openapi.yml
  format: yaml
  label: AppSkyline Metadata API
  slug: appskyline-com-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-metadata-api-openapi.yml
- filename: appskyline-com-review-status-api-openapi.yml
  format: yaml
  label: AppSkyline Review Status API
  slug: appskyline-com-review-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-review-status-api-openapi.yml
- filename: appskyline-com-sandbox-api-openapi.yml
  format: yaml
  label: AppSkyline Sandbox API
  slug: appskyline-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-sandbox-api-openapi.yml
- filename: appskyline-com-stats-api-openapi.yml
  format: yaml
  label: AppSkyline Stats API
  slug: appskyline-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-stats-api-openapi.yml
- filename: appskyline-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: AppSkyline Webhook subscriptions API
  slug: appskyline-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appskyline-com/openapi/appskyline-com-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appskyline.com
  spf: true
hosts:
- cert_expires: Dec 27 17:21:57 2026 GMT
  host: appskyline.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AppSkyline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppSkyline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppSkyline
provider_slug: appskyline-com
slug: appskyline-com-domain-security
source_filename: appskyline-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appskyline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 17:21:57 2026 GMT\n  hsts: false\ndomains:\n- domain: appskyline.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/appskyline-com/security/appskyline-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- App Store Optimization
- Analytics
- Marketing
- Software-as-a-Service
- Developer Tools
- Company
---
