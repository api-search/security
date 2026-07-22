---
api_specs:
- filename: workist-integrations-openapi-original.yml
  format: yaml
  label: Workist Integrations & Developer API
  slug: workist-integrations-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/openapi/workist-integrations-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workist.com
  spf: true
hosts:
- cert_expires: Oct  1 20:02:15 2026 GMT
  host: www.workist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 10:52:41 2026 GMT
  host: docs.workist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 09:39:47 2026 GMT
  host: api.workist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workist
provider_slug: workist
slug: workist-domain-security
source_filename: workist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.workist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 10:52:41 2026 GMT\n  hsts: false\n- host: api.workist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 09:39:47 2026 GMT\n  hsts: false\ndomains:\n- domain: workist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workist/refs/heads/main/security/workist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documents
- Document Processing
- Artificial Intelligence
- Automation
- Orders
- Invoices
- ERP
- B2B
- Master Data
---
