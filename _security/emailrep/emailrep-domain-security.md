---
api_specs:
- filename: emailrep-api-openapi.yml
  format: yaml
  label: EmailRep API
  slug: emailrep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/openapi/emailrep-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emailrep.io
  spf: false
hosts:
- cert_expires: Aug 20 10:35:56 2026 GMT
  host: emailrep.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Emailrep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EmailRep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: EmailRep
provider_slug: emailrep
slug: emailrep-domain-security
source_filename: emailrep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emailrep.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 20 10:35:56 2026 GMT\n  hsts: null\ndomains:\n- domain: emailrep.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emailrep/refs/heads/main/security/emailrep-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Security
- Email
- Email Reputation
- Threat Intelligence
- Phishing
- Fraud Prevention
- Anti-Abuse
- Deliverability
- Risk Scoring
- Public APIs
---
