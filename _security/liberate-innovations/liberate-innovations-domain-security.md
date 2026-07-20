---
api_specs:
- filename: liberate-innovations-orchestration-openapi.yml
  format: yaml
  label: Liberate Orchestration Platform API
  slug: orchestration-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/openapi/liberate-innovations-orchestration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liberateinc.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: liberateinc.io
  spf: false
hosts:
- cert_expires: Oct  3 00:13:52 2026 GMT
  host: www.liberateinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 01:50:36 2026 GMT
  host: docs.liberateinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: integration.liberateinc.io
  https: false
kind: domain-security
layout: security
method: probed
name: Liberate Innovations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liberate Innovations, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liberate Innovations
provider_slug: liberate-innovations
slug: liberate-innovations-domain-security
source_filename: liberate-innovations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liberateinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:13:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.liberateinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:50:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integration.liberateinc.io\n  https: false\ndomains:\n- domain: liberateinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: liberateinc.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberate-innovations/refs/heads/main/security/liberate-innovations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Artificial Intelligence
- Voice AI
- Conversational AI
- Workflow Orchestration
- Claims Automation
- Integration
- Contact Center
---
