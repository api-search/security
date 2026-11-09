---
api_specs:
- filename: brokervsadvisor-com-enquiry-api-openapi.yml
  format: yaml
  label: Broker vs Advisor Enquiry API
  slug: brokervsadvisor-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-enquiry-api-openapi.yml
- filename: brokervsadvisor-com-guide-api-openapi.yml
  format: yaml
  label: Broker vs Advisor Guide API
  slug: brokervsadvisor-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-guide-api-openapi.yml
- filename: brokervsadvisor-com-mcp-api-openapi.yml
  format: yaml
  label: Broker vs Advisor MCP API
  slug: brokervsadvisor-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brokervsadvisor-com/openapi/brokervsadvisor-com-mcp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brokervsadvisor.com
  spf: true
hosts:
- cert_expires: Jan 10 20:40:17 2027 GMT
  host: brokervsadvisor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brokervsadvisor Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Broker vs Advisor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Broker vs Advisor
provider_slug: brokervsadvisor-com
slug: brokervsadvisor-com-domain-security
source_filename: brokervsadvisor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brokervsadvisor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 20:40:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brokervsadvisor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/brokervsadvisor-com/security/brokervsadvisor-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business
- Finance
- Legal
- Advisory
- M&A
---
