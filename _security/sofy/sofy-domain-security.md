---
api_specs:
- filename: sofy-public-api-openapi.yml
  format: yaml
  label: SOFY Public API
  slug: sofy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofy/refs/heads/main/openapi/sofy-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sofy.ai
  spf: true
hosts:
- cert_expires: Dec 28 05:54:47 2026 GMT
  host: sofy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 15:54:06 2026 GMT
  host: docs.sofy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 05:54:47 2026 GMT
  host: public.sofy.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sofy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SOFY, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SOFY
provider_slug: sofy
slug: sofy-domain-security
source_filename: sofy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sofy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:54:47 2026 GMT\n  hsts: false\n- host: docs.sofy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:54:06 2026 GMT\n  hsts: false\n- host: public.sofy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 05:54:47 2026 GMT\n  hsts: null\ndomains:\n- domain: sofy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofy/refs/heads/main/security/sofy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- AI Testing
- Test Automation
- Mobile Testing
- QA
- No-Code
- Continuous Testing
- DevOps
---
