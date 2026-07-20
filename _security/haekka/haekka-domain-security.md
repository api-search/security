---
api_specs:
- filename: haekka-public-api-openapi.yml
  format: yaml
  label: Haekka Public API
  slug: haekka-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haekka/refs/heads/main/openapi/haekka-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: haekka.com
  spf: true
hosts:
- cert_expires: Aug 11 21:13:12 2026 GMT
  host: haekka.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 00:50:23 2026 GMT
  host: app.haekka.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haekka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haekka, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Haekka
provider_slug: haekka
slug: haekka-domain-security
source_filename: haekka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haekka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 21:13:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.haekka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 00:50:23 2026 GMT\n  hsts: null\ndomains:\n- domain: haekka.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haekka/refs/heads/main/security/haekka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security Awareness Training
- Compliance Training
- Microlearning
- Slack
- Phishing Simulation
- Employee Training
- HIPAA
- SOC 2
- API
---
