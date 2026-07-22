---
api_specs:
- filename: upsie-partner-network-openapi.yml
  format: yaml
  label: Upsie Partner Network API
  slug: upsie-partner-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upsie/refs/heads/main/openapi/upsie-partner-network-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upsie.com
  spf: false
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Oct  4 05:47:18 2026 GMT
  host: upsie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 05:47:18 2026 GMT
  host: api.upsie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upsie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upsie, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Upsie
provider_slug: upsie
slug: upsie-domain-security
source_filename: upsie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upsie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:47:18 2026 GMT\n  hsts: false\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upsie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:47:18 2026 GMT\n  hsts: false\ndomains:\n- domain: upsie.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upsie/refs/heads/main/security/upsie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Warranties
- Protection Plans
- Consumer Electronics
- Repairs
- Insurance
---
