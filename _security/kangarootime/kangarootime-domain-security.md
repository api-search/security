---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kangarootime.com
  spf: true
hosts:
- cert_expires: Oct 21 11:59:33 2026 GMT
  host: kangarootime.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kangarootime Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kangarootime, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kangarootime
provider_slug: kangarootime
slug: kangarootime-domain-security
source_filename: kangarootime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kangarootime.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 11:59:33 2026 GMT\n  hsts: false\ndomains:\n- domain: kangarootime.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kangarootime/refs/heads/main/security/kangarootime-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Childcare
- Early Childhood Education
- Education
- Child Care Management
- Enrollment
- Billing
- Payments
- Attendance
- Parent Communication
- Staff Management
- Business Intelligence
- Data Feeds
- Software-as-a-Service
---
