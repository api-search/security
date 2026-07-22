---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synaptic.build
  spf: true
hosts:
- cert_expires: Sep  1 10:32:46 2026 GMT
  host: www.synaptic.build
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synaptic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synaptic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Synaptic
provider_slug: synaptic
slug: synaptic-domain-security
source_filename: synaptic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synaptic.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:32:46 2026 GMT\n  hsts: false\ndomains:\n- domain: synaptic.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synaptic/refs/heads/main/security/synaptic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Salesforce
- Agentforce
- Healthcare
- Government
- Enterprise Software
- Consulting
---
