---
api_specs:
- filename: environmental-protection-agency-openapi.yml
  format: yaml
  label: EPA Envirofacts Data Service API
  slug: envirofacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/environmental-protection-agency/refs/heads/main/openapi/environmental-protection-agency-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: epa.gov
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.epa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: data.epa.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: aqs.epa.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Environmental Protection Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Environmental Protection Agency, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Environmental Protection Agency
provider_slug: environmental-protection-agency
slug: environmental-protection-agency-domain-security
source_filename: environmental-protection-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.epa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: aqs.epa.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: epa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/environmental-protection-agency/refs/heads/main/security/environmental-protection-agency-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Environment
- Federal Government
- Air Quality
- Open Data
---
