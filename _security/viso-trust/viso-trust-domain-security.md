---
api_specs:
- filename: viso-trust-openapi-original.json
  format: json
  label: VISO TRUST Client API
  slug: viso-trust-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/openapi/viso-trust-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: visotrust.com
  spf: true
hosts:
- cert_expires: Oct 10 04:23:27 2026 GMT
  host: visotrust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:05:48 2026 GMT
  host: app.visotrust.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viso Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VISO Trust, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: VISO Trust
provider_slug: viso-trust
slug: viso-trust-domain-security
source_filename: viso-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visotrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 04:23:27 2026 GMT\n  hsts: false\n- host: app.visotrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:05:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: visotrust.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viso-trust/refs/heads/main/security/viso-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Third Party Risk Management
- TPRM
- Vendor Risk
- Risk Management
- Compliance
- Cybersecurity
- Artificial Intelligence
---
