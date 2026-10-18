---
api_specs:
- filename: haptik-gccs-ws-api-openapi.yml
  format: yaml
  label: Haptik Gccs Ws API
  slug: haptik-gccs-ws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-gccs-ws-api-openapi.yml
- filename: haptik-haptik-api-api-openapi.yml
  format: yaml
  label: Haptik Haptik API
  slug: haptik-haptik-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-haptik-api-api-openapi.yml
- filename: haptik-integration-api-openapi.yml
  format: yaml
  label: Haptik Integration API
  slug: haptik-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-integration-api-openapi.yml
- filename: haptik-log-file-from-user-api-openapi.yml
  format: yaml
  label: Haptik Log File From User API
  slug: haptik-log-file-from-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-log-file-from-user-api-openapi.yml
- filename: haptik-mogambo-api-api-openapi.yml
  format: yaml
  label: Haptik Mogambo API
  slug: haptik-mogambo-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-mogambo-api-api-openapi.yml
- filename: haptik-user-api-openapi.yml
  format: yaml
  label: Haptik User API
  slug: haptik-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/openapi/haptik-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: haptik.ai
  spf: true
hosts:
- cert_expires: Nov 24 17:00:13 2026 GMT
  host: www.haptik.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Haptik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haptik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Haptik
provider_slug: haptik
slug: haptik-domain-security
source_filename: haptik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.haptik.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 17:00:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: haptik.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haptik/refs/heads/main/security/haptik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Messaging
- Enterprise
---
