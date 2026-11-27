---
api_specs:
- filename: kawaa-com-account-api-openapi.yml
  format: yaml
  label: kawaa-com Account API
  slug: kawaa-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-account-api-openapi.yml
- filename: kawaa-com-activity-api-openapi.yml
  format: yaml
  label: kawaa-com Activity API
  slug: kawaa-com-activity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-activity-api-openapi.yml
- filename: kawaa-com-api-keys-api-openapi.yml
  format: yaml
  label: kawaa-com API keys API
  slug: kawaa-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-api-keys-api-openapi.yml
- filename: kawaa-com-catalogue-api-openapi.yml
  format: yaml
  label: kawaa-com Catalogue API
  slug: kawaa-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-catalogue-api-openapi.yml
- filename: kawaa-com-deliverability-api-openapi.yml
  format: yaml
  label: kawaa-com Deliverability API
  slug: kawaa-com-deliverability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-deliverability-api-openapi.yml
- filename: kawaa-com-exports-api-openapi.yml
  format: yaml
  label: kawaa-com Exports API
  slug: kawaa-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-exports-api-openapi.yml
- filename: kawaa-com-health-api-openapi.yml
  format: yaml
  label: kawaa-com Health API
  slug: kawaa-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-health-api-openapi.yml
- filename: kawaa-com-jobs-api-openapi.yml
  format: yaml
  label: kawaa-com Jobs API
  slug: kawaa-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-jobs-api-openapi.yml
- filename: kawaa-com-search-api-openapi.yml
  format: yaml
  label: kawaa-com Search API
  slug: kawaa-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-search-api-openapi.yml
- filename: kawaa-com-verification-api-openapi.yml
  format: yaml
  label: kawaa-com Verification API
  slug: kawaa-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-verification-api-openapi.yml
- filename: kawaa-com-webhooks-api-openapi.yml
  format: yaml
  label: kawaa-com Webhooks API
  slug: kawaa-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kawaa-com/openapi/kawaa-com-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kawaa.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: kawaa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: kawaa-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for kawaa-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: kawaa-com
provider_slug: kawaa-com
slug: kawaa-com-domain-security
source_filename: kawaa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kawaa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kawaa.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kawaa-com/security/kawaa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Email Verification
- Software-as-a-Service
- Marketing
---
