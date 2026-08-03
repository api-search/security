---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carrumhealth.com
  spf: true
hosts:
- cert_expires: Oct 20 06:17:57 2026 GMT
  host: carrumhealth.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: my.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: core-service.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: care-service.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: message-service.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: price-service.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: upload-service.carrumhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:44 2026 GMT
  host: trust.carrumhealth.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carrum Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrum Health, probed live across 8 host(s) and 1 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carrum Health
provider_slug: carrum-health
slug: carrum-health-domain-security
source_filename: carrum-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 06:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: my.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: core-service.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: care-service.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: message-service.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: price-service.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: upload-service.carrumhealth.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: trust.carrumhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\nnotes: >-\n  The four additional *-service hosts and the trust center were probed directly on\n  2026-08-01 with the same TLS/HSTS method; none of the five API service hosts sets\n  Strict-Transport-Security, while the marketing host and the Vanta-hosted trust center\n  both do.\ndomains:\n- domain: carrumhealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrum-health/refs/heads/main/security/carrum-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Benefits
- Centers of Excellence
- Value-Based Care
- Bundled Payments
- Employee Benefits
- Surgery
- Care Navigation
- Digital Health
---
