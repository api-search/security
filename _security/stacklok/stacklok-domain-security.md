---
api_specs:
- filename: stacklok-toolhive-api-openapi.yml
  format: yaml
  label: ToolHive API
  slug: toolhive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-toolhive-api-openapi.yml
- filename: stacklok-registry-api-openapi.yml
  format: yaml
  label: ToolHive Registry API
  slug: toolhive-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/openapi/stacklok-registry-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:infra@stacklok.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stacklok.com
  spf: true
hosts:
- cert_expires: Oct 12 22:40:31 2026 GMT
  host: www.stacklok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stacklok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stacklok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Stacklok
provider_slug: stacklok
slug: stacklok-domain-security
source_filename: stacklok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stacklok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 22:40:31 2026 GMT\n  hsts: false\ndomains:\n- domain: stacklok.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:infra@stacklok.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacklok/refs/heads/main/security/stacklok-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Open Source
- MCP
- AI Agents
- API Governance
- Security
- Model Context Protocol
- Developer Tools
---
