---
api_specs:
- filename: logius-announce-api-openapi.yml
  format: yaml
  label: Logius Announce API
  slug: logius-announce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-announce-api-openapi.yml
- filename: logius-contracts-api-openapi.yml
  format: yaml
  label: Logius Contracts API
  slug: logius-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-contracts-api-openapi.yml
- filename: logius-domains-api-openapi.yml
  format: yaml
  label: Logius Domains API
  slug: logius-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-domains-api-openapi.yml
- filename: logius-events-api-openapi.yml
  format: yaml
  label: Logius Events API
  slug: logius-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-events-api-openapi.yml
- filename: logius-manager-api-openapi.yml
  format: yaml
  label: Logius Manager API
  slug: logius-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-manager-api-openapi.yml
- filename: logius-peers-api-openapi.yml
  format: yaml
  label: Logius Peers API
  slug: logius-peers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-peers-api-openapi.yml
- filename: logius-services-api-openapi.yml
  format: yaml
  label: Logius Services API
  slug: logius-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-services-api-openapi.yml
- filename: logius-subscriptions-api-openapi.yml
  format: yaml
  label: Logius Subscriptions API
  slug: logius-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-subscriptions-api-openapi.yml
- filename: logius-terugmelding-api-openapi.yml
  format: yaml
  label: Logius Terugmelding API
  slug: logius-terugmelding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmelding-api-openapi.yml
- filename: logius-terugmeldingstatus-api-openapi.yml
  format: yaml
  label: Logius Terugmelding Status API
  slug: logius-terugmeldingstatus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-terugmeldingstatus-api-openapi.yml
- filename: logius-token-api-openapi.yml
  format: yaml
  label: Logius Token API
  slug: logius-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-token-api-openapi.yml
- filename: logius-well-known-api-openapi.yml
  format: yaml
  label: Logius .well Known API
  slug: logius-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/openapi/logius-well-known-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "certsign.ro"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  - 0 issue "quovadisglobal.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: logius.nl
  spf: true
hosts:
- cert_expires: Oct 28 10:28:29 2026 GMT
  host: www.logius.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Logius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Logius
provider_slug: logius
slug: logius-domain-security
source_filename: logius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logius.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 10:28:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: logius.nl\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"certsign.ro\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logius/refs/heads/main/security/logius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Netherlands
- API Standards
- API Design Rules
- Digital Identity
- Data Exchange
- Public Sector
---
