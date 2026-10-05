---
api_specs:
- filename: datatheorem-llm-query-api-openapi.yml
  format: yaml
  label: Data Theorem Llm Query API
  slug: datatheorem-llm-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datatheorem/refs/heads/main/openapi/datatheorem-llm-query-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datatheorem.com
  spf: true
hosts:
- cert_expires: Dec 22 19:19:49 2026 GMT
  host: www.datatheorem.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datatheorem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data Theorem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Data Theorem
provider_slug: datatheorem
slug: datatheorem-domain-security
source_filename: datatheorem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datatheorem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 19:19:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: datatheorem.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datatheorem/refs/heads/main/security/datatheorem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Application Security
- API Security
- Cloud Security
- Mobile Security
---
