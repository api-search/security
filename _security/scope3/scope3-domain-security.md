---
api_specs:
- filename: scope3-measurement-openapi.yml
  format: yaml
  label: Scope3 Carbon Calculator (Measurement) API
  slug: scope3-carbon-calculator-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measurement-openapi.yml
- filename: scope3-ai-openapi-original.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scope3.com
  spf: true
hosts:
- cert_expires: Sep 30 21:56:56 2026 GMT
  host: scope3.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:01:28 2026 GMT
  host: api.scope3.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scope3 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scope3, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Scope3
provider_slug: scope3
slug: scope3-domain-security
source_filename: scope3-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scope3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:56:56 2026 GMT\n  hsts: false\n- host: api.scope3.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:01:28 2026 GMT\n  hsts: null\ndomains:\n- domain: scope3.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/security/scope3-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise
- Advertising
- Carbon Emissions
- Sustainability
- AdTech
- Measurement
- Artificial Intelligence
- Agentic
---
