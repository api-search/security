---
api_specs:
- filename: resistant-ai-documents-openapi.json
  format: json
  label: Resistant Documents API
  slug: resistant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-documents-openapi.json
- filename: resistant-ai-tenant-management-openapi.json
  format: json
  label: Resistant Documents Tenant Management API
  slug: resistant-documents-tenant-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/openapi/resistant-ai-tenant-management-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: resistant.ai
  spf: true
hosts:
- cert_expires: Sep 25 18:47:50 2026 GMT
  host: resistant.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resistant Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resistant AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Resistant AI
provider_slug: resistant-ai
slug: resistant-ai-domain-security
source_filename: resistant-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resistant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:47:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: resistant.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resistant-ai/refs/heads/main/security/resistant-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Fraud Detection
- Financial Crime
- Document Verification
- Document Forensics
- AML
- Identity Verification
- Fintech
- Machine Learning
---
