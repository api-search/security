---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appify.com
  spf: false
hosts:
- cert_expires: Oct 12 07:08:37 2026 GMT
  host: www.appify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:44:16 2026 GMT
  host: login.appify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appify, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Appify
provider_slug: appify
slug: appify-domain-security
source_filename: appify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 07:08:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: login.appify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appify.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appify/refs/heads/main/security/appify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Application Development
- No-Code
- Low-Code
- Enterprise Software
- Workflow-Automation
- Artificial Intelligence
- Integration
- Field Service
---
