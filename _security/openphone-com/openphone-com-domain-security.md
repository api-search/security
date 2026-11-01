---
api_specs:
- filename: openphone-com-openapi-generated.yml
  format: yaml
  label: Quo API
  slug: openphone-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openphone-com/openapi/_ae-authored/openphone-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openphone.com
  spf: true
hosts:
- cert_expires: Dec  7 02:22:51 2026 GMT
  host: www.openphone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openphone Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quo
provider_slug: openphone-com
slug: openphone-com-domain-security
source_filename: openphone-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openphone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:22:51 2026 GMT\n  hsts: false\ndomains:\n- domain: openphone.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/openphone-com/security/openphone-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Phone System
- Shared Numbers
- AI Agent
- Small Business
- Integrations
- CRM
- Call Routing
---
