---
api_specs:
- filename: guardr-io-openapi-generated.yml
  format: yaml
  label: Guardr API
  slug: guardr-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/guardr-io/openapi/_ae-authored/guardr-io-openapi-generated.yml
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
  dmarc_policy: quarantine
  dnssec: true
  domain: guardr.io
  spf: true
hosts:
- cert_expires: Jan 29 03:10:37 2027 GMT
  host: guardr.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Guardr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guardr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Guardr
provider_slug: guardr-io
slug: guardr-io-domain-security
source_filename: guardr-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guardr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 03:10:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guardr.io\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/guardr-io/security/guardr-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monitoring
- Uptime
- SSL
- Security
- Websites
---
