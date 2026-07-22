---
api_specs:
- filename: upguard-cyberrisk-openapi-original.json
  format: json
  label: UpGuard CyberRisk API
  slug: upguard-cyberrisk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/openapi/upguard-cyberrisk-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: upguard.com
  spf: true
hosts:
- cert_expires: Aug 29 23:33:50 2026 GMT
  host: www.upguard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 20:05:02 2026 GMT
  host: cyber-risk.upguard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpGuard, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: UpGuard
provider_slug: upguard
slug: upguard-domain-security
source_filename: upguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cyber-risk.upguard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:05:02 2026 GMT\n  hsts: null\ndomains:\n- domain: upguard.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upguard/refs/heads/main/security/upguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Third-Party Risk Management
- Attack Surface Management
- Vendor Risk
- Security Ratings
- Data Leaks
- Threat Intelligence
---
