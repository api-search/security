---
api_specs:
- filename: capepartners-fr-openapi.yml
  format: yaml
  label: Cape Partners Sniffer Agent API
  slug: cape-partners-sniffer-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capepartners-fr/refs/heads/main/openapi/capepartners-fr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capepartners.fr
  spf: false
hosts:
- cert_expires: Nov  7 12:57:52 2026 GMT
  host: capepartners.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capepartners Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cape Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cape Partners
provider_slug: capepartners-fr
slug: capepartners-fr-domain-security
source_filename: capepartners-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capepartners.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 12:57:52 2026 GMT\n  hsts: false\ndomains:\n- domain: capepartners.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capepartners-fr/refs/heads/main/security/capepartners-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Mergers and Acquisitions
- Deal Flow
- Valuation
- Investment
- Financial Services
- Agents
- A2A
- France
- Technology
- Software-as-a-Service
---
