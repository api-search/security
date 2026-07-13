---
api_specs:
- filename: saashub-openapi.yml
  format: yaml
  label: SaaSHub API
  slug: saashub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saashub/refs/heads/main/openapi/saashub-openapi.yml
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
  domain: saashub.com
  spf: true
hosts:
- cert_expires: Oct  7 06:09:24 2026 GMT
  host: www.saashub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saashub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SaaSHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SaaSHub
provider_slug: saashub
slug: saashub-domain-security
source_filename: saashub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saashub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 06:09:24 2026 GMT\n  hsts: null\ndomains:\n- domain: saashub.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saashub/refs/heads/main/security/saashub-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Alternatives
- SaaS
- Software Discovery
- Software Catalog
---
