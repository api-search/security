---
api_specs:
- filename: kleinanzeigen-openapi-generated.yml
  format: yaml
  label: Kleinanzeigen API
  slug: kleinanzeigen-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kleinanzeigen/openapi/_ae-authored/kleinanzeigen-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:kleinanzeigen-sre@adevinta.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kleinanzeigen.de
  spf: true
hosts:
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: kleinanzeigen.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kleinanzeigen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kleinanzeigen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kleinanzeigen
provider_slug: kleinanzeigen
slug: kleinanzeigen-domain-security
source_filename: kleinanzeigen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kleinanzeigen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kleinanzeigen.de\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:kleinanzeigen-sre@adevinta.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kleinanzeigen/security/kleinanzeigen-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- classifieds
- marketplace
- Germany
- free-ads
- consumer
---
