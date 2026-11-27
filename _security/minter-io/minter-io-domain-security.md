---
api_specs:
- filename: minter-io-openapi-generated.yml
  format: yaml
  label: Minterly Limited API
  slug: minter-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/minter-io/openapi/_ae-authored/minter-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:caa-violations@minter.io"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: minter.io
  spf: true
hosts:
- cert_expires: Jan 30 11:06:02 2027 GMT
  host: minter.io
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Minterly Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Minterly Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Minterly Limited
provider_slug: minter-io
slug: minter-io-domain-security
source_filename: minter-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: minter.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 11:06:02 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: minter.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:caa-violations@minter.io\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/minter-io/security/minter-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Social Media
- Analytics
- Software-as-a-Service
- Marketing
---
