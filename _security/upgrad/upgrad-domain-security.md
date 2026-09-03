---
api_specs:
- filename: upgrad-partner-openapi.yml
  format: yaml
  label: upGrad Partner Service API
  slug: upgrad-partner-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-partner-openapi.yml
- filename: upgrad-learner-analytics-openapi.yml
  format: yaml
  label: upGrad Learner Experience Analytics API
  slug: upgrad-learner-experience-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/openapi/upgrad-learner-analytics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upgrad.com
  spf: true
hosts:
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: www.upgrad.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:33:24 2026 GMT
  host: partner.upgrad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 20:53:06 2026 GMT
  host: learner-analytics-rest.upgrad.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upgrad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for upGrad, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: upGrad
provider_slug: upgrad
slug: upgrad-domain-security
source_filename: upgrad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upgrad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner.upgrad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:33:24 2026 GMT\n  hsts: null\n- host: learner-analytics-rest.upgrad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:53:06 2026 GMT\n  hsts: null\ndomains:\n- domain: upgrad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upgrad/refs/heads/main/security/upgrad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- EdTech
- Online Learning
- Higher Education
- Certification
- Learning Analytics
- Partner Management
- India
---
