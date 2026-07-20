---
api_specs:
- filename: captivateiq-openapi-original.yml
  format: yaml
  label: CaptivateIQ API
  slug: captivateiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/openapi/captivateiq-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: captivateiq.com
  spf: true
hosts:
- cert_expires: Sep 12 23:24:00 2026 GMT
  host: www.captivateiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 17:13:53 2026 GMT
  host: developers.captivateiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:56:12 2026 GMT
  host: api.captivateiq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Captivateiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CaptivateIQ, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CaptivateIQ
provider_slug: captivateiq
slug: captivateiq-domain-security
source_filename: captivateiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.captivateiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:24:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.captivateiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:13:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.captivateiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:56:12 2026 GMT\n  hsts: null\ndomains:\n- domain: captivateiq.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/captivateiq/refs/heads/main/security/captivateiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud Saas
- Sales Commissions
- Incentive Compensation Management
- Sales Performance Management
- Revenue Operations
- Finance
- Payouts
- Commission Plans
- Sales Compensation
---
