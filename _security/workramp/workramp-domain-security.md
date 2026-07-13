---
api_specs:
- filename: llms.txt
  format: yaml
  label: WorkRamp API
  slug: workramp-api
  spec_type: OpenAPI
  url: https://developers.workramp.com/llms.txt
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workramp.com
  spf: true
hosts:
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: www.workramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 22:16:36 2026 GMT
  host: developers.workramp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: app.workramp.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workramp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkRamp, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorkRamp
provider_slug: workramp
slug: workramp-domain-security
source_filename: workramp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.workramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:16:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.workramp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: workramp.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workramp/refs/heads/main/security/workramp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Learning Management
- Revenue Enablement
- Sales Enablement
- Training
- Onboarding
- LMS
- Assessments
- Certifications
- Coaching
- Go-to-Market
---
