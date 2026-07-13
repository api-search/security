---
api_specs:
- filename: policy-api.yml
  format: yaml
  label: Open Policy Agent Policy API
  slug: open-policy-agent-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/policy-api.yml
- filename: data-api.yml
  format: yaml
  label: Open Policy Agent Data API
  slug: open-policy-agent-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/data-api.yml
- filename: query-api.yml
  format: yaml
  label: Open Policy Agent Query API
  slug: open-policy-agent-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/query-api.yml
- filename: compile-api.yml
  format: yaml
  label: Open Policy Agent Compile API
  slug: open-policy-agent-compile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/compile-api.yml
- filename: health-api.yml
  format: yaml
  label: Open Policy Agent Health API
  slug: open-policy-agent-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/health-api.yml
- filename: config-api.yml
  format: yaml
  label: Open Policy Agent Config API
  slug: open-policy-agent-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/config-api.yml
- filename: status-api.yml
  format: yaml
  label: Open Policy Agent Status API
  slug: open-policy-agent-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/openapi/status-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openpolicyagent.org
  spf: false
hosts:
- cert_expires: Sep 18 19:18:56 2026 GMT
  host: www.openpolicyagent.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Policy Agent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Policy Agent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Policy Agent
provider_slug: open-policy-agent
slug: open-policy-agent-domain-security
source_filename: open-policy-agent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openpolicyagent.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 19:18:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openpolicyagent.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-policy-agent/refs/heads/main/security/open-policy-agent-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Policies
- Standards
---
