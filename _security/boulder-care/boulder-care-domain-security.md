---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: boulder.care
  spf: true
hosts:
- cert_expires: Sep 10 14:43:42 2026 GMT
  host: www.boulder.care
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:37:23 2026 GMT
  host: api.boulder.care
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Added by hand — this host is not referenced from apis.yml (Boulder Care publishes no API), but it is the live Apollo GraphQL backend for the patient mobile app and was found by STEP 0b contract discovery. /health returns HTTP 200 "ok".
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Boulder Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boulder Care, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Boulder Care
provider_slug: boulder-care
slug: boulder-care-domain-security
source_filename: boulder-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boulder.care\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:43:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.boulder.care\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 06:37:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: 'Added by hand — this host is not referenced from apis.yml (Boulder Care\n    publishes no API), but it is the live Apollo GraphQL backend for the patient\n    mobile app and was found by STEP 0b contract discovery. /health returns HTTP 200\n    \"ok\".'\ndomains:\n- domain: boulder.care\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boulder-care/refs/heads/main/security/boulder-care-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Telehealth
- Behavioral Health
- Addiction Treatment
- Substance Use Disorder
- Digital Health
- Medicaid
- Virtual Care
- Mobile Health
---
