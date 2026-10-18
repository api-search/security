---
api_specs:
- filename: composabl-reference-api-openapi.yml
  format: yaml
  label: Composabl Reference API
  slug: composabl-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/composabl/refs/heads/main/openapi/composabl-reference-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amesa.com
  spf: true
hosts:
- cert_expires: Dec 31 19:11:54 2026 GMT
  host: www.amesa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Composabl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Composabl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Composabl
provider_slug: composabl
slug: composabl-domain-security
source_filename: composabl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amesa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 19:11:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amesa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/composabl/refs/heads/main/security/composabl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Enterprise
- Automation
- Agents
- Platform
- Company
---
