---
api_specs:
- filename: trooth-co-legal-api-openapi.yml
  format: yaml
  label: Trooth Legal API
  slug: trooth-co-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-legal-api-openapi.yml
- filename: trooth-co-mobile-api-openapi.yml
  format: yaml
  label: Trooth Mobile API
  slug: trooth-co-mobile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-mobile-api-openapi.yml
- filename: trooth-co-network-api-openapi.yml
  format: yaml
  label: Trooth Network API
  slug: trooth-co-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-network-api-openapi.yml
- filename: trooth-co-problems-api-openapi.yml
  format: yaml
  label: Trooth Problems API
  slug: trooth-co-problems-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-problems-api-openapi.yml
- filename: trooth-co-public-mesh-api-openapi.yml
  format: yaml
  label: Trooth Public Mesh API
  slug: trooth-co-public-mesh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-public-mesh-api-openapi.yml
- filename: trooth-co-version-api-openapi.yml
  format: yaml
  label: Trooth Version API
  slug: trooth-co-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trooth-co/openapi/trooth-co-version-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: true
  domain: trooth.co
  spf: true
hosts:
- cert_expires: Jan  5 18:29:26 2027 GMT
  host: trooth.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trooth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trooth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trooth
provider_slug: trooth-co
slug: trooth-co-domain-security
source_filename: trooth-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trooth.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 18:29:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trooth.co\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/trooth-co/security/trooth-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Trust
- Infrastructure
- Cybersecurity
- AI
- Data
---
