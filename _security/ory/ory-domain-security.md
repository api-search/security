---
api_specs:
- filename: ory-hydra-openapi.json
  format: json
  label: Ory Hydra
  slug: hydra
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-hydra-openapi.json
- filename: ory-kratos-openapi.json
  format: json
  label: Ory Kratos
  slug: kratos
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-kratos-openapi.json
- filename: ory-keto-openapi.json
  format: json
  label: Ory Keto
  slug: keto
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-keto-openapi.json
- filename: ory-oathkeeper-openapi.json
  format: json
  label: Ory Oathkeeper
  slug: oathkeeper
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/openapi/ory-oathkeeper-openapi.json
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
  dmarc_policy: reject
  dnssec: false
  domain: ory.sh
  spf: true
hosts:
- cert_expires: Sep 23 04:28:42 2026 GMT
  host: www.ory.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ory
provider_slug: ory
slug: ory-domain-security
source_filename: ory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ory.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 04:28:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ory.sh\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ory/refs/heads/main/security/ory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- OAuth2
- OpenID Connect
- Open Source
---
