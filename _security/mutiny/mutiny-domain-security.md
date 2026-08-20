---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mutinyhq.com
  spf: true
hosts:
- cert_expires: Oct 24 09:30:55 2026 GMT
  host: www.mutinyhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: mcp.mutinyhq.com
  hsts: false
  https: true
  note: The MCP server host returns no Strict-Transport-Security header on any response (checked 2026-08-13 on GET and POST /mcp). It does set a Content-Security-Policy of "default-src 'self'; connect-src 'self' https://*.mutinyhq.com". This is the host that carries every authenticated agent call.
  tls_version: TLSv1.3
- host: status.mutinyhq.com
  https: false
  note: CNAMEs to Atlassian Statuspage (2c8f8lzxjbxr.stspg-customer.com) but presents CN=*.statuspage.io, which does not cover status.mutinyhq.com — TLS validation fails for every conforming client. See lifecycle/mutiny-lifecycle.yml.
  tls_error: certificate name mismatch
kind: domain-security
layout: security
method: probed
name: Mutiny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mutiny, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mutiny
provider_slug: mutiny
slug: mutiny-domain-security
source_filename: mutiny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mutinyhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 09:30:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.mutinyhq.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    The MCP server host returns no Strict-Transport-Security header on any response (checked 2026-08-13\n    on GET and POST /mcp). It does set a Content-Security-Policy of \"default-src 'self'; connect-src\n    'self' https://*.mutinyhq.com\". This is the host that carries every authenticated agent call.\n- host: status.mutinyhq.com\n  https: false\n  tls_error: certificate name mismatch\n  note: >-\n    CNAMEs to Atlassian Statuspage (2c8f8lzxjbxr.stspg-customer.com) but presents CN=*.statuspage.io,\n    which does not cover status.mutinyhq.com — TLS validation fails for every conforming client. See\n    lifecycle/mutiny-lifecycle.yml.\n\
  domains:\n- domain: mutinyhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutiny/refs/heads/main/security/mutiny-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Sales
- Marketing
- Go-To-Market
- Artificial Intelligence
- AI Agents
- Sales Enablement
- Account Based Marketing
- Workflow-Automation
- MCP
---
