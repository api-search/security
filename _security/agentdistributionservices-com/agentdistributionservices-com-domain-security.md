---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agentdistributionservices.com
  spf: false
hosts:
- cert_expires: Dec 27 00:38:43 2026 GMT
  host: agentdistributionservices.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentdistributionservices Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Distribution, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Agent Distribution
provider_slug: agentdistributionservices-com
slug: agentdistributionservices-com-domain-security
source_filename: agentdistributionservices-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdistributionservices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 00:38:43 2026 GMT\n  hsts: null\ndomains:\n- domain: agentdistributionservices.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agentdistributionservices-com/security/agentdistributionservices-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Agent Distribution
- MCP
- Preflight
- Pricing
---
