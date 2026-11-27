---
api_specs:
- filename: lumail-io-campaigns-api-openapi.yml
  format: yaml
  label: Lumail Campaigns API
  slug: lumail-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-campaigns-api-openapi.yml
- filename: lumail-io-domains-api-openapi.yml
  format: yaml
  label: Lumail Domains API
  slug: lumail-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-domains-api-openapi.yml
- filename: lumail-io-email-api-openapi.yml
  format: yaml
  label: Lumail Email API
  slug: lumail-io-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-email-api-openapi.yml
- filename: lumail-io-events-api-openapi.yml
  format: yaml
  label: Lumail Events API
  slug: lumail-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-events-api-openapi.yml
- filename: lumail-io-subscribers-api-openapi.yml
  format: yaml
  label: Lumail Subscribers API
  slug: lumail-io-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-subscribers-api-openapi.yml
- filename: lumail-io-tags-api-openapi.yml
  format: yaml
  label: Lumail Tags API
  slug: lumail-io-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-tags-api-openapi.yml
- filename: lumail-io-verify-api-openapi.yml
  format: yaml
  label: Lumail Verify API
  slug: lumail-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumail-io/openapi/lumail-io-verify-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lumail.io
  spf: true
hosts:
- cert_expires: Jan 11 09:14:19 2027 GMT
  host: lumail.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lumail
provider_slug: lumail-io
slug: lumail-io-domain-security
source_filename: lumail-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumail.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 09:14:19 2027 GMT\n  hsts: false\ndomains:\n- domain: lumail.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lumail-io/security/lumail-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Email Marketing
- Automation
- Software-as-a-Service
---
