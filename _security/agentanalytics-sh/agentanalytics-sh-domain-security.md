---
api_specs:
- filename: agentanalytics-sh-api-openapi.yml
  format: yaml
  label: Agent Analytics API API
  slug: agent-analytics-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentanalytics-sh/openapi/_original/agentanalytics-sh-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agentanalytics.sh
  spf: true
hosts:
- cert_expires: Dec 30 11:44:39 2026 GMT
  host: agentanalytics.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentanalytics Sh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Analytics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agent Analytics
provider_slug: agentanalytics-sh
slug: agentanalytics-sh-domain-security
source_filename: agentanalytics-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentanalytics.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 11:44:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentanalytics.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agentanalytics-sh/security/agentanalytics-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Artificial Intelligence
- Web Analytics
- Open Source
- Software-as-a-Service
---
