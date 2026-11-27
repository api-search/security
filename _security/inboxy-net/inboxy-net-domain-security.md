---
api_specs:
- filename: inboxy-net-account-api-openapi.yml
  format: yaml
  label: Inboxy Account API
  slug: inboxy-net-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-account-api-openapi.yml
- filename: inboxy-net-addresses-api-openapi.yml
  format: yaml
  label: Inboxy Addresses API
  slug: inboxy-net-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-addresses-api-openapi.yml
- filename: inboxy-net-api-keys-api-openapi.yml
  format: yaml
  label: Inboxy API keys API
  slug: inboxy-net-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-api-keys-api-openapi.yml
- filename: inboxy-net-articles-api-openapi.yml
  format: yaml
  label: Inboxy Articles API
  slug: inboxy-net-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-articles-api-openapi.yml
- filename: inboxy-net-attachments-api-openapi.yml
  format: yaml
  label: Inboxy Attachments API
  slug: inboxy-net-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-attachments-api-openapi.yml
- filename: inboxy-net-billing-api-openapi.yml
  format: yaml
  label: Inboxy Billing API
  slug: inboxy-net-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-billing-api-openapi.yml
- filename: inboxy-net-domains-api-openapi.yml
  format: yaml
  label: Inboxy Domains API
  slug: inboxy-net-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-domains-api-openapi.yml
- filename: inboxy-net-feeds-api-openapi.yml
  format: yaml
  label: Inboxy Feeds API
  slug: inboxy-net-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-feeds-api-openapi.yml
- filename: inboxy-net-mail-api-openapi.yml
  format: yaml
  label: Inboxy Mail API
  slug: inboxy-net-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-mail-api-openapi.yml
- filename: inboxy-net-messages-api-openapi.yml
  format: yaml
  label: Inboxy Messages API
  slug: inboxy-net-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-messages-api-openapi.yml
- filename: inboxy-net-outbox-api-openapi.yml
  format: yaml
  label: Inboxy Outbox API
  slug: inboxy-net-outbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-outbox-api-openapi.yml
- filename: inboxy-net-service-api-openapi.yml
  format: yaml
  label: Inboxy Service API
  slug: inboxy-net-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-service-api-openapi.yml
- filename: inboxy-net-webhooks-api-openapi.yml
  format: yaml
  label: Inboxy Webhooks API
  slug: inboxy-net-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inboxy-net/openapi/inboxy-net-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@inboxy.net"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: inboxy.net
  spf: true
hosts:
- cert_expires: Jan  6 01:11:01 2027 GMT
  host: inboxy.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inboxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inboxy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Inboxy
provider_slug: inboxy-net
slug: inboxy-net-domain-security
source_filename: inboxy-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inboxy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 01:11:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inboxy.net\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@inboxy.net\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/inboxy-net/security/inboxy-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Email Alias
- Browser Extension
- Daily Digest
---
