---
api_specs:
- filename: centml-openapi.yml
  format: yaml
  label: CentML Serverless Inference (Chat Completions) API
  slug: centml-serverless-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Models API
  slug: centml-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Deployments / Endpoints API
  slug: centml-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
- filename: centml-openapi.yml
  format: yaml
  label: CentML Clusters API
  slug: centml-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/openapi/centml-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centml.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: centml.com
  spf: false
hosts:
- host: centml.ai
  https: false
- cert_expires: Aug 31 21:40:01 2026 GMT
  host: docs.centml.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 00:55:09 2026 GMT
  host: api.centml.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Centml Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CentML, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CentML
provider_slug: centml
slug: centml-domain-security
source_filename: centml-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: centml.ai\n  https: false\n- host: docs.centml.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:40:01 2026 GMT\n  hsts: false\n- host: api.centml.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:55:09 2026 GMT\n  hsts: null\ndomains:\n- domain: centml.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: centml.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centml/refs/heads/main/security/centml-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Inference
- Serverless
- GPU
---
