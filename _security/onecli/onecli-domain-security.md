---
api_specs:
- filename: onecli-openapi-original.yml
  format: yaml
  label: OneCLI API
  slug: onecli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onecli/refs/heads/main/openapi/onecli-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onecli.sh
  spf: true
hosts:
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: onecli.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: api.onecli.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onecli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onecli, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Onecli
provider_slug: onecli
slug: onecli-domain-security
source_filename: onecli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onecli.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.onecli.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: onecli.sh\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onecli/refs/heads/main/security/onecli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Identity
- AI Agents
- Secrets Management
- Credentials
- Gateway
- OAuth
- Developer Tools
- MCP
- Vault
---
