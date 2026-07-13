---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stepci.com
  spf: true
hosts:
- cert_expires: Aug 17 06:07:04 2026 GMT
  host: stepci.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Step Ci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Step CI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Step CI
provider_slug: step-ci
slug: step-ci-domain-security
source_filename: step-ci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stepci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:07:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stepci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/step-ci/refs/heads/main/security/step-ci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Testing
- Functional Testing
- Testing
- CI/CD
- Quality Assurance
- Automation
- Open Source
---
