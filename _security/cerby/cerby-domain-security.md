---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cerby.com
  spf: true
hosts:
- cert_expires: Sep 28 02:21:28 2026 GMT
  host: www.cerby.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: developer.cerby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: my-workspace.cerby.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cerby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cerby, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cerby
provider_slug: cerby
slug: cerby-domain-security
source_filename: cerby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cerby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:21:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cerby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: false\n- host: my-workspace.cerby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cerby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerby/refs/heads/main/security/cerby-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity
- Access Management
- Security
- Password Management
- Provisioning
- SCIM
- Identity Governance
- Nonfederated Applications
- Automation
- Webhook
---
