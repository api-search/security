---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coreview.com
  spf: true
hosts:
- cert_expires: Oct 14 14:32:33 2026 GMT
  host: www.coreview.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 09:01:27 2026 GMT
  host: help.coreview.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 09:01:27 2026 GMT
  host: apiproxy.coreview.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coreview Fka 4Ward365 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoreView (FKA 4ward365), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CoreView (FKA 4ward365)
provider_slug: coreview-fka-4ward365
slug: coreview-fka-4ward365-domain-security
source_filename: coreview-fka-4ward365-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 14:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.coreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:01:27 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apiproxy.coreview.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:01:27 2026 GMT\n  hsts: null\ndomains:\n- domain: coreview.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coreview-fka-4ward365/refs/heads/main/security/coreview-fka-4ward365-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Microsoft 365
- SaaS Management
- Governance
- Security
- Identity
- Automation
- Workflow
- License Management
- IT Operations
---
