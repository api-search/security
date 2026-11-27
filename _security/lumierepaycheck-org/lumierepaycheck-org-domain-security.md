---
api_specs:
- filename: lumierepaycheck-org-monitoring-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Monitoring API
  slug: lumierepaycheck-org-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-monitoring-api-openapi.yml
- filename: lumierepaycheck-org-security-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Security API
  slug: lumierepaycheck-org-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-security-api-openapi.yml
- filename: lumierepaycheck-org-trust-api-openapi.yml
  format: yaml
  label: Lumière PayCheck Trust API
  slug: lumierepaycheck-org-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lumierepaycheck-org/openapi/lumierepaycheck-org-trust-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lumierepaycheck.org
  spf: true
hosts:
- cert_expires: Dec 25 22:22:57 2026 GMT
  host: lumierepaycheck.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lumière PayCheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumière PayCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lumière PayCheck
provider_slug: lumierepaycheck-org
slug: lumierepaycheck-org-domain-security
source_filename: lumierepaycheck-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumierepaycheck.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 22:22:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumierepaycheck.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lumierepaycheck-org/security/lumierepaycheck-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Payments
- Automation
- Agents
---
