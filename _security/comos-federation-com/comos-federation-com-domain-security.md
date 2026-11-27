---
api_specs:
- filename: comos-federation-com-openapi.yml
  format: yaml
  label: ComOS Federation Gateway
  slug: comos-federation-gateway
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comos-federation-com/openapi/comos-federation-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: comos-federation.com
  spf: true
hosts:
- cert_expires: Jan  9 18:55:55 2027 GMT
  host: comos-federation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ComOS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ComOS
provider_slug: comos-federation-com
slug: comos-federation-com-domain-security
source_filename: comos-federation-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: comos-federation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 18:55:55 2027 GMT\n  hsts: false\ndomains:\n- domain: comos-federation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/comos-federation-com/security/comos-federation-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Commerce
- AI Agents
- MCP
- Federation
- Payments
- Self-Hosted
- Operating System
---
