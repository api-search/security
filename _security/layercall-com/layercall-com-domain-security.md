---
api_specs:
- filename: layercall-com-ai-agents-api-openapi.yml
  format: yaml
  label: layercall-com AI agents API
  slug: layercall-com-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-ai-agents-api-openapi.yml
- filename: layercall-com-batch-api-openapi.yml
  format: yaml
  label: layercall-com Batch API
  slug: layercall-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-batch-api-openapi.yml
- filename: layercall-com-device-api-openapi.yml
  format: yaml
  label: layercall-com Device API
  slug: layercall-com-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-device-api-openapi.yml
- filename: layercall-com-reputation-api-openapi.yml
  format: yaml
  label: layercall-com Reputation API
  slug: layercall-com-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-reputation-api-openapi.yml
- filename: layercall-com-rules-api-openapi.yml
  format: yaml
  label: layercall-com Rules API
  slug: layercall-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-rules-api-openapi.yml
- filename: layercall-com-scoring-api-openapi.yml
  format: yaml
  label: layercall-com Scoring API
  slug: layercall-com-scoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-scoring-api-openapi.yml
- filename: layercall-com-unified-api-openapi.yml
  format: yaml
  label: layercall-com Unified API
  slug: layercall-com-unified-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layercall-com/openapi/layercall-com-unified-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: layercall.com
  spf: true
hosts:
- cert_expires: Dec 21 03:21:58 2026 GMT
  host: layercall.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Layercall Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for layercall-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: layercall-com
provider_slug: layercall-com
slug: layercall-com-domain-security
source_filename: layercall-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layercall.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 03:21:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: layercall.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/layercall-com/security/layercall-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FraudDetection
- TrustIntelligence
- API
- Security
---
