---
api_specs:
- filename: fast-io-openapi-generated.yml
  format: yaml
  label: Fastio API
  slug: fast-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fast-io/openapi/_ae-authored/fast-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fast.io
  spf: true
hosts:
- cert_expires: Jan 10 17:35:21 2027 GMT
  host: fast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fastio
provider_slug: fast-io
slug: fast-io-domain-security
source_filename: fast-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 17:35:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fast.io\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fast-io/security/fast-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Cloud Storage
- Collaboration
- Enterprise
- Productivity
---
