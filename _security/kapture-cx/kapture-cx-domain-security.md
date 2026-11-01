---
api_specs:
- filename: kapture-cx-openapi-generated.yml
  format: yaml
  label: Kapture CX API
  slug: kapture-cx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kapture-cx/openapi/_ae-authored/kapture-cx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kapture.cx
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: kapture.cx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kapture Cx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kapture CX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kapture CX
provider_slug: kapture-cx
slug: kapture-cx-domain-security
source_filename: kapture-cx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kapture.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kapture.cx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kapture-cx/security/kapture-cx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Customer Experience
- CRM
- AI
- Automation
- Contact Center
---
