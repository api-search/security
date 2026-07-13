---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pinwheelapi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpinwheel.com
  spf: true
hosts:
- cert_expires: Aug 17 03:44:34 2026 GMT
  host: pinwheelapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: api.getpinwheel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:42:27 2026 GMT
  host: docs.pinwheelapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pinwheel Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pinwheel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Pinwheel
provider_slug: pinwheel-api
slug: pinwheel-api-domain-security
source_filename: pinwheel-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pinwheelapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 03:44:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.getpinwheel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: null\n- host: docs.pinwheelapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pinwheelapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: getpinwheel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinwheel-api/refs/heads/main/security/pinwheel-api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employment
- Income
- Payroll
- Direct Deposit
- Identity
- Verification
- Financial
- Tax
- Bill Pay
---
