---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fireflyhealth.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: firefly.health
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.fireflyhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: members.firefly.health
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  csp: true
  host: api-prod.firefly.health
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: HSTS/CSP observed on a follow-up HEAD of https://api-prod.firefly.health/ on 2026-08-01; the automated probe recorded null.
  server: gunicorn
  tls_version: TLSv1.2
  x_content_type_options: nosniff
  x_frame_options: DENY
kind: domain-security
layout: security
method: probed
name: Firefly Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firefly Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Firefly Health
provider_slug: firefly-health
slug: firefly-health-domain-security
source_filename: firefly-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fireflyhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: members.firefly.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\n- host: api-prod.firefly.health\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: gunicorn\n  csp: true\n  x_frame_options: DENY\n  x_content_type_options: nosniff\n  note: 'HSTS/CSP observed on a follow-up HEAD of https://api-prod.firefly.health/ on\n    2026-08-01; the automated probe recorded null.'\ndomains:\n- domain: fireflyhealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: firefly.health\n  dnssec: true\n  caa:\n  - 0 issue \"\
  amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firefly-health/refs/heads/main/security/firefly-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Plans
- Virtual Care
- Primary Care
- Telehealth
- Health Insurance
- Employee Benefits
- Digital Health
---
