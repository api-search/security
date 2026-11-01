---
api_specs:
- filename: openapi.json
  format: json
  label: The Water Hub API
  slug: thewaterhub-api
  spec_type: OpenAPI
  url: https://thewaterhub.org/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thewaterhub.org
  spf: true
hosts:
- cert_expires: Jan 15 11:35:39 2027 GMT
  host: thewaterhub.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Thewaterhub Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for thewaterhub-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: thewaterhub-org
provider_slug: thewaterhub-org
slug: thewaterhub-org-domain-security
source_filename: thewaterhub-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thewaterhub.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 11:35:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thewaterhub.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/thewaterhub-org/security/thewaterhub-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Water
- Pricing
- Dataset
- API
---
