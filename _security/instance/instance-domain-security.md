---
api_specs:
- filename: instance-verifier-openapi.json
  format: json
  label: Robot Rollout Verifier API
  slug: robot-rollout-verifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instance/refs/heads/main/openapi/instance-verifier-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: instancelabs.ai
  spf: false
hosts:
- cert_expires: Oct  6 05:17:00 2026 GMT
  host: www.instancelabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:17:00 2026 GMT
  host: demo.instancelabs.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Instance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Instance
provider_slug: instance
slug: instance-domain-security
source_filename: instance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.instancelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.instancelabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:17:00 2026 GMT\n  hsts: null\ndomains:\n- domain: instancelabs.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instance/refs/heads/main/security/instance-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Machine Learning
- Verification
- Evaluation
- Data Quality
- Artificial Intelligence
- Y Combinator
---
