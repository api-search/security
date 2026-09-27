---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog;cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: averlon.ai
  spf: true
hosts:
- cert_expires: Dec 13 11:17:20 2026 GMT
  host: www.averlon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Averlon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Averlon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Averlon
provider_slug: averlon
slug: averlon-domain-security
source_filename: averlon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.averlon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 11:17:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: averlon.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog;cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/averlon/refs/heads/main/security/averlon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Security
- AI
- Vulnerability Management
- Automation
---
