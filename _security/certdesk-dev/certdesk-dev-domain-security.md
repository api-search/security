---
api_specs:
- filename: certdesk-dev-certificate-api-openapi.yml
  format: yaml
  label: certdesk-dev Certificate API
  slug: certdesk-dev-certificate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-certificate-api-openapi.yml
- filename: certdesk-dev-dns-api-openapi.yml
  format: yaml
  label: certdesk-dev Dns API
  slug: certdesk-dev-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-dns-api-openapi.yml
- filename: certdesk-dev-dns-info-api-openapi.yml
  format: yaml
  label: certdesk-dev Dns Info API
  slug: certdesk-dev-dns-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-dns-info-api-openapi.yml
- filename: certdesk-dev-expiry-api-openapi.yml
  format: yaml
  label: certdesk-dev Expiry API
  slug: certdesk-dev-expiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-expiry-api-openapi.yml
- filename: certdesk-dev-explain-api-openapi.yml
  format: yaml
  label: certdesk-dev Explain API
  slug: certdesk-dev-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-explain-api-openapi.yml
- filename: certdesk-dev-security-api-openapi.yml
  format: yaml
  label: certdesk-dev Security API
  slug: certdesk-dev-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-security-api-openapi.yml
- filename: certdesk-dev-watch-api-openapi.yml
  format: yaml
  label: certdesk-dev Watch API
  slug: certdesk-dev-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/certdesk-dev/openapi/certdesk-dev-watch-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: certdesk.dev
  spf: true
hosts:
- cert_expires: Dec 17 04:01:49 2026 GMT
  host: certdesk.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certdesk Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for certdesk-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: certdesk-dev
provider_slug: certdesk-dev
slug: certdesk-dev-domain-security
source_filename: certdesk-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certdesk.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 04:01:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: certdesk.dev\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/certdesk-dev/security/certdesk-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
