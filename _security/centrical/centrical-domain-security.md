---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centrical.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dmarc_rua: dmarc-reports@centrical.me
  dnssec: false
  domain: centrical.me
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:spf.mandrillapp.com include:mail.zendesk.com -all
hosts:
- cert_expires: Sep 30 12:47:49 2026 GMT
  host: centrical.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 300
  https: true
  note: HSTS max-age of 300s is effectively non-protective.
  role: marketing site (WordPress)
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: api.centrical.me
  hsts: false
  hsts_max_age: null
  https: true
  note: No Strict-Transport-Security header on the API host.
  role: production API host (AWS API Gateway, us-east-1)
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: app.centrical.me
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: tenant customer application (CloudFront)
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: docs.centrical.me
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: tenant customer application (CloudFront)
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: powerup.centrical.me
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: mobile/PowerUp client SPA (CloudFront)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centrical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centrical, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Centrical
provider_slug: centrical
slug: centrical-domain-security
source_filename: centrical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The centrical.com row is written by 0-working/probe-domain-security.py from apis.yml. The\n  centrical.me rows were measured by hand on 2026-08-10 with the same method (openssl s_client for\n  TLS version and cert expiry, HEAD for HSTS, dig for DS/CAA/SPF/DMARC) after a DNS sweep found\n  Centrical's production application and API hosts on its second domain, which apis.yml does not\n  reference. Two findings worth naming: centrical.com sets an HSTS max-age of only 300 seconds\n  (5 minutes), which is far too short to offer real protection and below the 31536000 the\n  centrical.me app hosts use; and api.centrical.me — the production API host — sends no HSTS header\n  at all. Neither domain publishes DNSSEC or CAA.\n\nhosts:\n- host: centrical.com\n  role: marketing site (WordPress)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:47:49 2026 GMT\n\
  \  hsts: true\n  hsts_max_age: 300\n  hsts_include_subdomains: false\n  note: HSTS max-age of 300s is effectively non-protective.\n- host: api.centrical.me\n  role: production API host (AWS API Gateway, us-east-1)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M01\n  hsts: false\n  hsts_max_age: null\n  note: No Strict-Transport-Security header on the API host.\n- host: app.centrical.me\n  role: tenant customer application (CloudFront)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: docs.centrical.me\n  role: tenant customer application (CloudFront)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: powerup.centrical.me\n  role: mobile/PowerUp client SPA (CloudFront)\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n\ndomains:\n- domain: centrical.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: centrical.me\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: 'v=spf1 include:spf.protection.outlook.com include:spf.mandrillapp.com include:mail.zendesk.com -all'\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_rua: dmarc-reports@centrical.me\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrical/refs/heads/main/security/centrical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Employee Engagement
- Performance Management
- Gamification
- Microlearning
- Contact Center
- Workforce Engagement Management
- Coaching
- Quality Management
- Human Resources
- Software-as-a-Service
---
