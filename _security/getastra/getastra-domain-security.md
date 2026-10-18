---
api_specs:
- filename: getastra-openapi-generated.yml
  format: yaml
  label: Astra Pentest API
  slug: getastra-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/getastra/refs/heads/main/openapi/_ae-authored/getastra-openapi-generated.yml
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
  domain: getastra.com
  spf: true
hosts:
- cert_expires: Jan 14 13:11:23 2027 GMT
  host: getastra.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Getastra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astra Pentest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Astra Pentest
provider_slug: getastra
slug: getastra-domain-security
source_filename: getastra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getastra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 13:11:23 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getastra.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getastra/refs/heads/main/security/getastra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- PenetrationTesting
- API
- Cloud
---
