---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: axtria.com
  spf: true
hosts:
- cert_expires: Aug  7 10:24:49 2026 GMT
  host: www.axtria.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 04:25:19 2026 GMT
  host: docs.axtria.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: 'product documentation host; HTTP Basic auth gated (401, WWW-Authenticate: Basic realm="docs.axtria.com")'
  tls_version: TLSv1.3
- cert_expires: Feb 11 11:02:44 2027 GMT
  host: insights.axtria.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: HubSpot-hosted content/asset host (hubfs) used for the blog and resource library
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axtria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axtria, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Axtria
provider_slug: axtria
slug: axtria-domain-security
source_filename: axtria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axtria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  7 10:24:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.axtria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 04:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: 'product documentation host; HTTP Basic auth gated (401, WWW-Authenticate:\n    Basic realm=\"docs.axtria.com\")'\n- host: insights.axtria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 11:02:44 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: HubSpot-hosted content/asset host (hubfs) used for the blog and resource library\ndomains:\n- domain: axtria.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axtria/refs/heads/main/security/axtria-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Pharmaceuticals
- Analytics
- Data Management
- Artificial Intelligence
- Sales Operations
- Marketing
- Cloud Software
- Healthcare
- Commercial Operations
---
