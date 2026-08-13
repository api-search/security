---
api_specs:
- filename: endeavor-biomedicines-wordpress-rest-openapi.yml
  format: yaml
  label: Endeavor BioMedicines WordPress REST API
  slug: endeavor-biomedicines-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/openapi/endeavor-biomedicines-wordpress-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: endeavorbiomedicines.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: endeavorbiomedicines.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endeavor Biomedicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endeavor BioMedicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Endeavor BioMedicines
provider_slug: endeavor-biomedicines
slug: endeavor-biomedicines-domain-security
source_filename: endeavor-biomedicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endeavorbiomedicines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: endeavorbiomedicines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavor-biomedicines/refs/heads/main/security/endeavor-biomedicines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Clinical Trials
- Healthcare
- Drug Development
- Content
- WordPress
---
