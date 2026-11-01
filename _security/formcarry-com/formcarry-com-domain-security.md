---
api_specs:
- filename: formcarry-com-api-openapi-generated.yml
  format: yaml
  label: formcarry-com api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formcarry-com/openapi/_ae-authored/formcarry-com-api-openapi-generated.yml
- filename: formcarry-com-api-reference-openapi-generated.yml
  format: yaml
  label: formcarry-com api reference API
  slug: api-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formcarry-com/openapi/_ae-authored/formcarry-com-api-reference-openapi-generated.yml
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
  dmarc_policy: none
  dnssec: false
  domain: formcarry.com
  spf: true
hosts:
- cert_expires: Jan  1 15:44:33 2027 GMT
  host: formcarry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formcarry Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for formcarry-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: formcarry-com
provider_slug: formcarry-com
slug: formcarry-com-domain-security
source_filename: formcarry-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formcarry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 15:44:33 2027 GMT\n  hsts: false\ndomains:\n- domain: formcarry.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/formcarry-com/security/formcarry-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- API
- Forms
- Backend-as-a-Service
- Webhooks
---
