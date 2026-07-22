---
api_specs:
- filename: workspace-openapi-original.json
  format: json
  label: VSCO Workspace API
  slug: vsco-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vsco/refs/heads/main/openapi/workspace-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:ops@vsco.co"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vsco.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tave.io
  spf: true
hosts:
- cert_expires: Sep 30 21:00:29 2026 GMT
  host: www.vsco.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: tave.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 17:14:47 2026 GMT
  host: workspace.vsco.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vsco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VSCO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: VSCO
provider_slug: vsco
slug: vsco-domain-security
source_filename: vsco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vsco.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 21:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tave.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: workspace.vsco.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:14:47 2026 GMT\n  hsts: null\ndomains:\n- domain: vsco.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:ops@vsco.co\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tave.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vsco/refs/heads/main/security/vsco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Photography
- Photo Editing
- Creative Community
- Studio Management
- SaaS
---
