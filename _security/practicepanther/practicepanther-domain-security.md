---
api_specs:
- filename: practicepanther-practicepanther-api-openapi.yml
  format: yaml
  label: PracticePanther API
  slug: practicepanther-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/practicepanther/refs/heads/main/openapi/practicepanther-practicepanther-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: practicepanther.com
  spf: true
hosts:
- cert_expires: Aug 18 09:43:25 2026 GMT
  host: www.practicepanther.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:01:28 2026 GMT
  host: support.practicepanther.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 15:12:10 2026 GMT
  host: app.practicepanther.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Practicepanther Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PracticePanther, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PracticePanther
provider_slug: practicepanther
slug: practicepanther-domain-security
source_filename: practicepanther-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.practicepanther.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 09:43:25 2026 GMT\n  hsts: false\n- host: support.practicepanther.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:01:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: app.practicepanther.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 15:12:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: practicepanther.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/practicepanther/refs/heads/main/security/practicepanther-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Law Practice Management
- Case Management
- Billing
- Trust Accounting
- Time Tracking
- Legal Tech
---
