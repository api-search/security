---
description: ''
domains:
- caa:
  - d28d4f8xatasfu.cloudfront.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: briefcase.so
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: briefcase.so
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Briefcase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Briefcase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Briefcase
provider_slug: briefcase
slug: briefcase-domain-security
source_filename: briefcase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: briefcase.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: briefcase.so\n  dnssec: true\n  caa:\n  - d28d4f8xatasfu.cloudfront.net.\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/briefcase/refs/heads/main/security/briefcase-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Accounting
- Bookkeeping
- Fintech
- Artificial Intelligence
- Automation
- VAT Compliance
- Agentic AI
- SaaS
- United Kingdom
---
