---
api_specs:
- filename: appsmith-openapi.yaml
  format: yaml
  label: Appsmith API
  slug: appsmith-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/openapi/appsmith-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: appsmith.com
  spf: true
hosts:
- cert_expires: Sep 26 21:18:33 2026 GMT
  host: www.appsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 15:57:13 2026 GMT
  host: docs.appsmith.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: app.appsmith.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appsmith, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Appsmith
provider_slug: appsmith
slug: appsmith-domain-security
source_filename: appsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 21:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.appsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 15:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.appsmith.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: appsmith.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmith/refs/heads/main/security/appsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Low-Code
- Open Source
- Internal Tools
- Workflow Automation
- Developer Tools
---
