---
api_specs:
- filename: rootline-core-openapi-generated.yml
  format: yaml
  label: Rootline core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-core-openapi-generated.yml
- filename: rootline-in-person-payments-openapi-generated.yml
  format: yaml
  label: Rootline in person payments API
  slug: in-person-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-in-person-payments-openapi-generated.yml
- filename: rootline-payments-openapi-generated.yml
  format: yaml
  label: Rootline payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-payments-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 iodef "mailto:caa-violations@rootline.com"
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rootline.com
  spf: true
hosts:
- cert_expires: Jan 15 22:35:25 2027 GMT
  host: rootline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rootline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rootline, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Rootline
provider_slug: rootline
slug: rootline-domain-security
source_filename: rootline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rootline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 22:35:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rootline.com\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 iodef \"mailto:caa-violations@rootline.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/rootline/security/rootline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- FinTech
- EmbeddedPayments
- API
- Platform
---
