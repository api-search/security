---
api_specs:
- filename: lakpura-com-authentication-api-openapi.yml
  format: yaml
  label: Lakpura Authentication API
  slug: lakpura-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-authentication-api-openapi.yml
- filename: lakpura-com-customers-api-openapi.yml
  format: yaml
  label: Lakpura Customers API
  slug: lakpura-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-customers-api-openapi.yml
- filename: lakpura-com-jobs-api-openapi.yml
  format: yaml
  label: Lakpura Jobs API
  slug: lakpura-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-jobs-api-openapi.yml
- filename: lakpura-com-notifications-api-openapi.yml
  format: yaml
  label: Lakpura Notifications API
  slug: lakpura-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-notifications-api-openapi.yml
- filename: lakpura-com-users-api-openapi.yml
  format: yaml
  label: Lakpura Users API
  slug: lakpura-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lakpura-com/openapi/lakpura-com-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lakpura.com
  spf: true
hosts:
- cert_expires: Feb  1 19:46:53 2027 GMT
  host: lakpura.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lakpura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lakpura, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lakpura
provider_slug: lakpura-com
slug: lakpura-com-domain-security
source_filename: lakpura-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lakpura.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 19:46:53 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: lakpura.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lakpura-com/security/lakpura-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- E-Commerce
- IT Services
- Sri Lanka
- Marketplace
---
