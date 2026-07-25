---
api_specs:
- filename: adaptive-security-audit-logs-api-openapi.yml
  format: yaml
  label: Adaptive Security Audit Logs API
  slug: adaptive-security-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-audit-logs-api-openapi.yml
- filename: adaptive-security-groups-api-openapi.yml
  format: yaml
  label: Adaptive Security Groups API
  slug: adaptive-security-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-groups-api-openapi.yml
- filename: adaptive-security-phishing-api-openapi.yml
  format: yaml
  label: Adaptive Security Phishing API
  slug: adaptive-security-phishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-phishing-api-openapi.yml
- filename: adaptive-security-training-api-openapi.yml
  format: yaml
  label: Adaptive Security Training API
  slug: adaptive-security-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-training-api-openapi.yml
- filename: adaptive-security-users-api-openapi.yml
  format: yaml
  label: Adaptive Security Users API
  slug: adaptive-security-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/openapi/adaptive-security-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adaptivesecurity.com
  spf: true
hosts:
- cert_expires: Oct  8 16:09:39 2026 GMT
  host: www.adaptivesecurity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.adaptivesecurity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api.adaptivesecurity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adaptive Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adaptive Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adaptive Security
provider_slug: adaptive-security
slug: adaptive-security-domain-security
source_filename: adaptive-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adaptivesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 16:09:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.adaptivesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.adaptivesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: adaptivesecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adaptive-security/refs/heads/main/security/adaptive-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Security Awareness Training
- Phishing Simulation
- Deepfake Defense
- AI Governance
- Social Engineering
- Reporting
- Compliance
---
