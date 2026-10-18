---
api_specs:
- filename: contextgem-systemone-api-openapi.yml
  format: yaml
  label: ContextGem Systemone API
  slug: contextgem-systemone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contextgem/refs/heads/main/openapi/contextgem-systemone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contextgem.dev
  spf: true
hosts:
- cert_expires: Jan 12 20:55:26 2027 GMT
  host: contextgem.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contextgem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContextGem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ContextGem
provider_slug: contextgem
slug: contextgem-domain-security
source_filename: contextgem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contextgem.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 20:55:26 2027 GMT\n  hsts: false\ndomains:\n- domain: contextgem.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contextgem/refs/heads/main/security/contextgem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Natural Language Processing
- Data Extraction
- LLM
- Platform
- Company
---
