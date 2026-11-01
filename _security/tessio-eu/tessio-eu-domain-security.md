---
api_specs:
- filename: tessio-eu-age-verification-api-openapi.yml
  format: yaml
  label: tessio-eu Age Verification API
  slug: tessio-eu-age-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-age-verification-api-openapi.yml
- filename: tessio-eu-stats-api-openapi.yml
  format: yaml
  label: tessio-eu Stats API
  slug: tessio-eu-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-stats-api-openapi.yml
- filename: tessio-eu-webhooks-api-openapi.yml
  format: yaml
  label: tessio-eu Webhooks API
  slug: tessio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tessio.eu
  spf: true
hosts:
- cert_expires: Jan 24 08:35:22 2027 GMT
  host: tessio.eu
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tessio Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tessio-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: tessio-eu
provider_slug: tessio-eu
slug: tessio-eu-domain-security
source_filename: tessio-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tessio.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:35:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: tessio.eu\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tessio-eu/security/tessio-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AgeVerification
- EU
- API
- Identity
---
