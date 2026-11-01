---
api_specs:
- filename: worklytics-openapi-generated.yml
  format: yaml
  label: Worklytics API
  slug: worklytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/worklytics/openapi/_ae-authored/worklytics-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: worklytics.co
  spf: true
hosts:
- cert_expires: Nov 28 18:45:37 2026 GMT
  host: www.worklytics.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Worklytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Worklytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Worklytics
provider_slug: worklytics
slug: worklytics-domain-security
source_filename: worklytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.worklytics.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 18:45:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: worklytics.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/worklytics/security/worklytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Analytics
- Workplace
- AI
- Productivity
---
