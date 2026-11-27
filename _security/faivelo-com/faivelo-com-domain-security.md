---
api_specs:
- filename: faivelo-com-core-openapi-generated.yml
  format: yaml
  label: Faivelo core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-core-openapi-generated.yml
- filename: faivelo-com-transactional-openapi-generated.yml
  format: yaml
  label: Faivelo transactional API
  slug: transactional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-transactional-openapi-generated.yml
- filename: faivelo-com-v1-openapi-generated.yml
  format: yaml
  label: Faivelo v1 API
  slug: v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-v1-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: faivelo.com
  spf: true
hosts:
- cert_expires: Jan 14 03:32:08 2027 GMT
  host: faivelo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faivelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faivelo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Faivelo
provider_slug: faivelo-com
slug: faivelo-com-domain-security
source_filename: faivelo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faivelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 03:32:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: faivelo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/faivelo-com/security/faivelo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Email
- Transactional Email
- Marketing Email
- Email API
- AI Agents
---
