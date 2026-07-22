---
api_specs:
- filename: serval-auth-openapi.yml
  format: yaml
  label: Serval Public API
  slug: serval-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/openapi/serval-auth-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: serval.com
  spf: true
hosts:
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.serval.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 22:32:57 2026 GMT
  host: docs.serval.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: public.api.serval.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Serval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serval, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Serval
provider_slug: serval
slug: serval-domain-security
source_filename: serval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.serval.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.serval.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 22:32:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: public.api.serval.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: serval.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serval/refs/heads/main/security/serval-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IT Service Management
- ITSM
- Help Desk
- Workflow Automation
- AI Agents
- Access Management
- Employee Support
- Ticketing
---
