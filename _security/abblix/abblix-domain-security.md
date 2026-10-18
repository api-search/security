---
api_specs:
- filename: abblix-connect-api-openapi.yml
  format: yaml
  label: Abblix Connect API
  slug: abblix-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abblix/refs/heads/main/openapi/abblix-connect-api-openapi.yml
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
  dmarc_policy: reject
  dnssec: true
  domain: abblix.com
  spf: true
hosts:
- cert_expires: Jan  4 21:28:16 2027 GMT
  host: www.abblix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abblix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abblix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Abblix
provider_slug: abblix
slug: abblix-domain-security
source_filename: abblix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abblix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 21:28:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abblix.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abblix/refs/heads/main/security/abblix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Identity
- OpenID Connect
- Authentication
- .NET
- Shared Signals
---
