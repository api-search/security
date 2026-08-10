---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brace.ai
  spf: true
hosts:
- cert_expires: Sep 15 15:06:55 2026 GMT
  host: brace.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brace
provider_slug: brace
slug: brace-domain-security
source_filename: brace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brace.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:06:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brace.ai\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brace/refs/heads/main/security/brace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mortgage
- Mortgage Servicing
- Loss Mitigation
- Default Servicing
- Financial Services
- Fintech
- Real Estate
- Workflow Automation
- Acquired
---
