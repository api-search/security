---
api_specs:
- filename: kion-cloud-operations-api-openapi.yml
  format: yaml
  label: Kion Cloud Operations API
  slug: kion-cloud-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/openapi/kion-cloud-operations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kion.io
  spf: true
hosts:
- cert_expires: Oct  6 08:32:36 2026 GMT
  host: kion.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:41:44 2026 GMT
  host: support.kion.io
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kion
provider_slug: kion
slug: kion-domain-security
source_filename: kion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:32:36 2026 GMT\n  hsts: false\n- host: support.kion.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:41:44 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: kion.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kion/refs/heads/main/security/kion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Operations
- Compliance
- Costs
- FinOps
- Governance
- Spend
---
