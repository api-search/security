---
api_specs:
- filename: oximy-public-api-openapi.yml
  format: yaml
  label: Oximy Public API
  slug: oximy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oximy/refs/heads/main/openapi/oximy-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oximy.com
  spf: true
hosts:
- cert_expires: Oct 10 05:28:28 2026 GMT
  host: api.oximy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oximy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oximy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oximy
provider_slug: oximy
slug: oximy-domain-security
source_filename: oximy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.oximy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 05:28:28 2026 GMT\n  hsts: null\ndomains:\n- domain: oximy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oximy/refs/heads/main/security/oximy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Governance
- LLM Observability
- AI Adoption
- Telemetry
- Policy Enforcement
- Artificial Intelligence
- Developer Tools
---
