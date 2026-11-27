---
api_specs:
- filename: rms-openapi.yml
  format: yaml
  label: Risk Modeler API
  slug: risk-modeler-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rms/openapi/rms-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: rms.com
  spf: true
hosts:
- cert_expires: Dec 13 07:27:52 2026 GMT
  host: www.rms.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Moody's RMS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moody''s RMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Moody's RMS
provider_slug: rms
slug: rms-domain-security
source_filename: rms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:27:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rms.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/rms/security/rms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Risk Management
- Modeling
- Analytics
- Technology
- Company
---
