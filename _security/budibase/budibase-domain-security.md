---
api_specs:
- filename: openapi.json
  format: json
  label: Budibase REST API
  slug: budibase-rest-api
  spec_type: OpenAPI
  url: https://budibase.com/api/public/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: budibase.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: budibase.app
  spf: false
hosts:
- cert_expires: Oct  7 15:20:34 2026 GMT
  host: budibase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 14:13:34 2026 GMT
  host: docs.budibase.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:17:26 2026 GMT
  host: budibase.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Budibase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Budibase, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Budibase
provider_slug: budibase
slug: budibase-domain-security
source_filename: budibase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: budibase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 15:20:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.budibase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 14:13:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: budibase.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: budibase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: budibase.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/security/budibase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Automation
- Internal Tools
- Low-Code
- Open Source
- Workflow Automation
---
