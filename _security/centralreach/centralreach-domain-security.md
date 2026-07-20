---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centralreach.com
  spf: true
hosts:
- cert_expires: Sep 25 01:51:20 2026 GMT
  host: centralreach.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: partners-api.centralreach.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centralreach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CentralReach, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CentralReach
provider_slug: centralreach
slug: centralreach-domain-security
source_filename: centralreach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centralreach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:51:20 2026 GMT\n  hsts: false\n- host: partners-api.centralreach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: centralreach.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centralreach/refs/heads/main/security/centralreach-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- ABA Therapy
- Autism
- IDD
- EMR
- Practice Management
- Behavioral Health
- Special Education
- Billing
- OAuth
---
