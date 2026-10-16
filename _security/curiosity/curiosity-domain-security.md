---
api_specs:
- filename: curiosity-openapi-generated.yml
  format: yaml
  label: Curiosity API
  slug: curiosity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/openapi/_ae-authored/curiosity-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curiosity.ai
  spf: true
hosts:
- cert_expires: Jan  7 17:54:10 2027 GMT
  host: curiosity.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curiosity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curiosity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curiosity
provider_slug: curiosity
slug: curiosity-domain-security
source_filename: curiosity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curiosity.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 17:54:10 2027 GMT\n  hsts: false\ndomains:\n- domain: curiosity.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curiosity/refs/heads/main/security/curiosity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Knowledge-Graph
- Enterprise
- Data-Integration
- On-Premises
- Company
---
