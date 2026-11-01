---
api_specs:
- filename: sudomock-com-account-api-openapi.yml
  format: yaml
  label: sudomock-com Account API
  slug: sudomock-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-account-api-openapi.yml
- filename: sudomock-com-background-removal-api-openapi.yml
  format: yaml
  label: sudomock-com Background removal API
  slug: sudomock-com-background-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-background-removal-api-openapi.yml
- filename: sudomock-com-fonts-api-openapi.yml
  format: yaml
  label: sudomock-com Fonts API
  slug: sudomock-com-fonts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-fonts-api-openapi.yml
- filename: sudomock-com-jobs-api-openapi.yml
  format: yaml
  label: sudomock-com Jobs API
  slug: sudomock-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-jobs-api-openapi.yml
- filename: sudomock-com-photo-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com Photo mockups API
  slug: sudomock-com-photo-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-photo-mockups-api-openapi.yml
- filename: sudomock-com-psd-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com PSD mockups API
  slug: sudomock-com-psd-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-psd-mockups-api-openapi.yml
- filename: sudomock-com-studio-api-openapi.yml
  format: yaml
  label: sudomock-com Studio API
  slug: sudomock-com-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-studio-api-openapi.yml
- filename: sudomock-com-video-mockups-api-openapi.yml
  format: yaml
  label: sudomock-com Video mockups API
  slug: sudomock-com-video-mockups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-video-mockups-api-openapi.yml
- filename: sudomock-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: sudomock-com Webhook deliveries API
  slug: sudomock-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-webhook-deliveries-api-openapi.yml
- filename: sudomock-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: sudomock-com Webhook endpoints API
  slug: sudomock-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sudomock-com/openapi/sudomock-com-webhook-endpoints-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: sudomock.com
  spf: true
hosts:
- cert_expires: Jan 16 23:14:51 2027 GMT
  host: sudomock.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sudomock Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for sudomock-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: sudomock-com
provider_slug: sudomock-com
slug: sudomock-com-domain-security
source_filename: sudomock-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sudomock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:14:51 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sudomock.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/sudomock-com/security/sudomock-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Mockup
- API
- PSD
- E-commerce
- Automation
---
