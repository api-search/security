---
api_specs:
- filename: pterodactyl-admin-api-openapi.yml
  format: yaml
  label: Pterodactyl Admin API
  slug: pterodactyl-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-admin-api-openapi.yml
- filename: pterodactyl-application-api-openapi.yml
  format: yaml
  label: Pterodactyl Application API
  slug: pterodactyl-application-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-application-api-openapi.yml
- filename: pterodactyl-client-api-openapi.yml
  format: yaml
  label: Pterodactyl Client API
  slug: pterodactyl-client-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-client-api-openapi.yml
- filename: pterodactyl-gpg-api-openapi.yml
  format: yaml
  label: Pterodactyl Gpg API
  slug: pterodactyl-gpg-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-gpg-api-openapi.yml
- filename: pterodactyl-installer-api-openapi.yml
  format: yaml
  label: Pterodactyl Installer API
  slug: pterodactyl-installer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-installer-api-openapi.yml
- filename: pterodactyl-pterodactyl-api-api-openapi.yml
  format: yaml
  label: Pterodactyl Pterodactyl API
  slug: pterodactyl-pterodactyl-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-pterodactyl-api-api-openapi.yml
- filename: pterodactyl-pterodactyl-api-openapi.yml
  format: yaml
  label: Pterodactyl Pterodactyl API
  slug: pterodactyl-pterodactyl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-pterodactyl-api-openapi.yml
- filename: pterodactyl-setup-22-api-openapi.yml
  format: yaml
  label: Pterodactyl Setup 22 API
  slug: pterodactyl-setup-22-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pterodactyl/openapi/pterodactyl-setup-22-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pterodactyl.io
  spf: true
hosts:
- cert_expires: Jan  3 20:31:12 2027 GMT
  host: pterodactyl.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pterodactyl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pterodactyl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pterodactyl
provider_slug: pterodactyl
slug: pterodactyl-domain-security
source_filename: pterodactyl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pterodactyl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 20:31:12 2027 GMT\n  hsts: false\ndomains:\n- domain: pterodactyl.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pterodactyl/security/pterodactyl-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Game Server
- Open Source
- Docker
- API
---
