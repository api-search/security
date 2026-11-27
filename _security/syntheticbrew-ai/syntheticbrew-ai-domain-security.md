---
api_specs:
- filename: syntheticbrew-ai-getting-started-openapi-generated.yml
  format: yaml
  label: SyntheticBrew getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-getting-started-openapi-generated.yml
- filename: syntheticbrew-ai-integration-openapi-generated.yml
  format: yaml
  label: SyntheticBrew integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-integration-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    agents: []
    checked: '2026-11-25'
    index:
    - alpn:
      - h2
      - http/1.1
      target: syntheticbrew.ai
    published: true
  dnssec: true
  domain: syntheticbrew.ai
  spf: true
hosts:
- cert_expires: Feb 11 20:17:20 2027 GMT
  host: syntheticbrew.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SyntheticBrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SyntheticBrew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SyntheticBrew
provider_slug: syntheticbrew-ai
slug: syntheticbrew-ai-domain-security
source_filename: syntheticbrew-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syntheticbrew.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 20:17:20 2027 GMT\n  hsts: false\ndomains:\n- domain: syntheticbrew.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-25'\n    published: true\n    index:\n    - target: syntheticbrew.ai\n      alpn:\n      - h2\n      - http/1.1\n    agents: []\n"
source_yaml_url: https://artifacts.apis.io/syntheticbrew-ai/security/syntheticbrew-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI
- Infrastructure
- Enterprise
- Agents
- NoCode
---
