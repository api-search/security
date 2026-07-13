---
api_specs:
- filename: webhooks-asyncapi.yml
  format: yaml
  label: Instatus
  slug: instatus
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/instatus/refs/heads/main/webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: instatus.com
  spf: true
hosts:
- cert_expires: Aug 18 08:12:26 2026 GMT
  host: instatus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instatus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instatus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Instatus
provider_slug: instatus
slug: instatus-domain-security
source_filename: instatus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instatus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 08:12:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: instatus.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instatus/refs/heads/main/security/instatus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business
- Public APIs
---
