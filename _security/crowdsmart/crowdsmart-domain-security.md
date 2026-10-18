---
api_specs:
- filename: crowdsmart-agents-api-openapi.yml
  format: yaml
  label: CrowdSmart Agents API
  slug: crowdsmart-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowdsmart/refs/heads/main/openapi/crowdsmart-agents-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: crowdsmart.ai
  spf: false
hosts:
- cert_expires: Jan  9 08:12:25 2027 GMT
  host: crowdsmart.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowdsmart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrowdSmart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CrowdSmart
provider_slug: crowdsmart
slug: crowdsmart-domain-security
source_filename: crowdsmart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdsmart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 08:12:25 2027 GMT\n  hsts: false\ndomains:\n- domain: crowdsmart.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdsmart/refs/heads/main/security/crowdsmart-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Governance
- TrustLayer
- CollectiveIntelligence
- Platform
---
