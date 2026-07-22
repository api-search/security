---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forwardplatform.com
  spf: true
hosts:
- cert_expires: Oct 15 01:27:26 2026 GMT
  host: forwardplatform.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forward Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forward Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forward Platform
provider_slug: forward-platform
slug: forward-platform-domain-security
source_filename: forward-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forwardplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 01:27:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: forwardplatform.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forward-platform/refs/heads/main/security/forward-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GovTech
- Government
- Nonprofits
- Foundations
- Program Management
- Case Management
- Payments
- Public Sector
- Service Delivery
---
