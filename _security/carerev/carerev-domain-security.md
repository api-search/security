---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carerev.com
  spf: true
hosts:
- cert_expires: Sep 10 14:05:14 2026 GMT
  host: www.carerev.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 20:47:07 2026 GMT
  host: api.carerev.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carerev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareRev, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CareRev
provider_slug: carerev
slug: carerev-domain-security
source_filename: carerev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carerev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.carerev.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 20:47:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carerev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carerev/refs/heads/main/security/carerev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Systems
- Workforce Management
- Staffing
- Nursing
- Marketplace
- Scheduling
- Human Resources
- Labor Marketplace
---
