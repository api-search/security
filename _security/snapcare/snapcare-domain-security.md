---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snapcare.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hiive.com
  spf: true
hosts:
- cert_expires: Nov  6 09:48:12 2026 GMT
  host: snapcare.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 05:37:55 2026 GMT
  host: www.hiive.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapCare, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SnapCare
provider_slug: snapcare
slug: snapcare-domain-security
source_filename: snapcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 09:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: www.hiive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:37:55 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: snapcare.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hiive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapcare/refs/heads/main/security/snapcare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Staffing
- Workforce Management
- Scheduling
- Marketplace
- Human Resources
- Nursing
---
