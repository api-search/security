---
api_specs:
- filename: sana-openapi.yml
  format: yaml
  label: Sana API
  slug: sana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/openapi/sana-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sanalabs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sana.ai
  spf: true
hosts:
- cert_expires: Sep 16 04:13:46 2026 GMT
  host: www.sanalabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: docs.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:49:35 2026 GMT
  host: app.sana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sana, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sana
provider_slug: sana
slug: sana-domain-security
source_filename: sana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sanalabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\n- host: app.sana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:49:35 2026 GMT\n  hsts: null\ndomains:\n- domain: sanalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sana/refs/heads/main/security/sana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise AI
- Artificial Intelligence
- Learning Management
- LMS
- Knowledge Management
- Agents
- SCIM
- xAPI
- REST API
---
