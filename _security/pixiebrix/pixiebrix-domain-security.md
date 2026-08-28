---
api_specs:
- filename: pixiebrix-openapi.yml
  format: yaml
  label: PixieBrix Developer API
  slug: pixiebrix-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixiebrix/refs/heads/main/openapi/pixiebrix-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pixiebrix.com
  spf: true
hosts:
- cert_expires: Oct 31 04:54:06 2026 GMT
  host: www.pixiebrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 20:22:42 2026 GMT
  host: docs.pixiebrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 04:49:52 2026 GMT
  host: app.pixiebrix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixiebrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PixieBrix, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PixieBrix
provider_slug: pixiebrix
slug: pixiebrix-domain-security
source_filename: pixiebrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pixiebrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 04:54:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.pixiebrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 20:22:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.pixiebrix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 04:49:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pixiebrix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixiebrix/refs/heads/main/security/pixiebrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Browser Extensions
- Low-Code
- Automation
- Artificial Intelligence
- Customer Support
- Enterprise Operations
- Workflow Automation
- Agent Governance
- Robotic Process Automation
---
