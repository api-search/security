---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zushealth.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: zusapi.com
  spf: false
hosts:
- cert_expires: Aug 24 09:33:49 2026 GMT
  host: docs.zushealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: api.zusapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: fqs.zusapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zus Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zus Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zus Health
provider_slug: zus-health
slug: zus-health-domain-security
source_filename: zus-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.zushealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 09:33:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zusapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: fqs.zusapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zushealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: zusapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zus-health/refs/heads/main/security/zus-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- FHIR
- Interoperability
- Health Data
- Patient Records
- EHR
- GraphQL
- Webhooks
---
