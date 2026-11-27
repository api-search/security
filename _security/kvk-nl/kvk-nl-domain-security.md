---
api_specs:
- filename: kvk-nl-abonnement-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Abonnement API
  slug: kvk-nl-abonnement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-abonnement-api-openapi.yml
- filename: kvk-nl-basisprofiel-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Basisprofiel API
  slug: kvk-nl-basisprofiel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-basisprofiel-api-openapi.yml
- filename: kvk-nl-naamgeving-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Naamgeving API
  slug: kvk-nl-naamgeving-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-naamgeving-api-openapi.yml
- filename: kvk-nl-signaal-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Signaal API
  slug: kvk-nl-signaal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-signaal-api-openapi.yml
- filename: kvk-nl-vestigingsprofiel-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Vestigingsprofiel API
  slug: kvk-nl-vestigingsprofiel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-vestigingsprofiel-api-openapi.yml
- filename: kvk-nl-zoeken-api-openapi.yml
  format: yaml
  label: Kamer van Koophandel (KVK) Zoeken API
  slug: kvk-nl-zoeken-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kvk-nl/openapi/kvk-nl-zoeken-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "quovadisglobal.com"
  - 0 issuewild ";"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kvk.nl
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: developers.kvk.nl
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kamer van Koophandel (KVK) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kamer van Koophandel (KVK), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kamer van Koophandel (KVK)
provider_slug: kvk-nl
slug: kvk-nl-domain-security
source_filename: kvk-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.kvk.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: kvk.nl\n  dnssec: true\n  caa:\n  - 0 issue \"quovadisglobal.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kvk-nl/security/kvk-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Register
- Government
- Netherlands
- Company Data
- KYC
- Open Data
---
