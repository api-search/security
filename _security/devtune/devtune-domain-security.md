---
api_specs:
- filename: devtune-accuracy-api-openapi.yml
  format: yaml
  label: DevTune Accuracy API
  slug: devtune-accuracy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-accuracy-api-openapi.yml
- filename: devtune-actions-api-openapi.yml
  format: yaml
  label: DevTune Actions API
  slug: devtune-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-actions-api-openapi.yml
- filename: devtune-adoption-api-openapi.yml
  format: yaml
  label: DevTune Adoption API
  slug: devtune-adoption-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-adoption-api-openapi.yml
- filename: devtune-agent-picks-api-openapi.yml
  format: yaml
  label: DevTune Agent Picks API
  slug: devtune-agent-picks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agent-picks-api-openapi.yml
- filename: devtune-agent-registration-api-openapi.yml
  format: yaml
  label: DevTune Agent registration API
  slug: devtune-agent-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agent-registration-api-openapi.yml
- filename: devtune-agents-api-openapi.yml
  format: yaml
  label: DevTune Agents API
  slug: devtune-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-agents-api-openapi.yml
- filename: devtune-ai-traffic-api-openapi.yml
  format: yaml
  label: DevTune AI Traffic API
  slug: devtune-ai-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-ai-traffic-api-openapi.yml
- filename: devtune-audit-and-pages-api-openapi.yml
  format: yaml
  label: DevTune Audit and pages API
  slug: devtune-audit-and-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-audit-and-pages-api-openapi.yml
- filename: devtune-citations-api-openapi.yml
  format: yaml
  label: DevTune Citations API
  slug: devtune-citations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-citations-api-openapi.yml
- filename: devtune-connection-and-usage-api-openapi.yml
  format: yaml
  label: DevTune Connection and usage API
  slug: devtune-connection-and-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-connection-and-usage-api-openapi.yml
- filename: devtune-content-gaps-api-openapi.yml
  format: yaml
  label: DevTune Content gaps API
  slug: devtune-content-gaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-content-gaps-api-openapi.yml
- filename: devtune-dex-api-openapi.yml
  format: yaml
  label: DevTune Dex API
  slug: devtune-dex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-dex-api-openapi.yml
- filename: devtune-library-and-knowledge-api-openapi.yml
  format: yaml
  label: DevTune Library and Knowledge API
  slug: devtune-library-and-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-library-and-knowledge-api-openapi.yml
- filename: devtune-positioning-api-openapi.yml
  format: yaml
  label: DevTune Positioning API
  slug: devtune-positioning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-positioning-api-openapi.yml
- filename: devtune-prompts-and-topics-api-openapi.yml
  format: yaml
  label: DevTune Prompts and topics API
  slug: devtune-prompts-and-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-prompts-and-topics-api-openapi.yml
- filename: devtune-results-api-openapi.yml
  format: yaml
  label: DevTune Results API
  slug: devtune-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-results-api-openapi.yml
- filename: devtune-setup-api-openapi.yml
  format: yaml
  label: DevTune Setup API
  slug: devtune-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-setup-api-openapi.yml
- filename: devtune-visibility-api-openapi.yml
  format: yaml
  label: DevTune Visibility API
  slug: devtune-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-visibility-api-openapi.yml
- filename: devtune-webhooks-api-openapi.yml
  format: yaml
  label: DevTune Webhooks API
  slug: devtune-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/devtune/openapi/devtune-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: devtune.ai
  spf: true
hosts:
- cert_expires: Jan 30 06:46:51 2027 GMT
  host: devtune.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DevTune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DevTune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DevTune
provider_slug: devtune
slug: devtune-domain-security
source_filename: devtune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devtune.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 06:46:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: devtune.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/devtune/security/devtune-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Search
- Analytics
- Platform
---
