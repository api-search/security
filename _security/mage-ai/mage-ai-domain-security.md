---
api_specs:
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Triggers & Runs API
  slug: pipeline-triggers-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipelines API
  slug: pipelines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Blocks API
  slug: blocks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Schedules API
  slug: schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mage.ai
  spf: true
hosts:
- cert_expires: Sep 26 08:53:39 2026 GMT
  host: www.mage.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 09:01:06 2026 GMT
  host: docs.mage.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mage Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mage, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mage
provider_slug: mage-ai
slug: mage-ai-domain-security
source_filename: mage-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:53:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:01:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mage.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/security/mage-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Pipelines
- Orchestration
- ETL
- Data Engineering
- Open Source
---
