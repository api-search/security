---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: arine.io
  spf: true
hosts:
- cert_expires: Oct  7 01:22:20 2026 GMT
  host: www.arine.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: api.arine.io
  hsts: false
  https: true
  note: AWS API Gateway; every probed path returns HTTP 403 ForbiddenException to anonymous callers
  tls_version: TLSv1.3
- cert_expires: Oct 12 23:59:59 2026 GMT
  host: app.arine.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 20 02:36:30 2026 GMT
  host: docs.arine.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:52:56 2026 GMT
  host: blog.arine.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 14:34:31 2026 GMT
  host: go.arine.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arine, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Arine
provider_slug: arine
slug: arine-domain-security
source_filename: arine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:22:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.arine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: false\n  note: AWS API Gateway; every probed path returns HTTP 403 ForbiddenException to\n    anonymous callers\n- host: app.arine.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: docs.arine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 02:36:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: blog.arine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:52:56 2026 GMT\n  hsts: true\n\
  \  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: go.arine.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 14:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arine.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nfindings:\n- No CAA records published for arine.io — any CA may issue for the domain.\n- DMARC policy is p=quarantine rather than p=reject.\n- No /.well-known/security.txt (RFC 9116) on any Arine host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arine/refs/heads/main/security/arine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health Care
- Medication Management
- Pharmacy
- Artificial Intelligence
- Clinical Decision Support
- Health Plans
- Population Health
- Value Based Care
- SaaS
---
