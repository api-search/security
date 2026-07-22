---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: symmetrical.ai
  spf: true
hosts:
- cert_expires: Aug 30 11:42:10 2026 GMT
  host: symmetrical.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Symmetrical Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symmetrical, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Symmetrical
provider_slug: symmetrical
slug: symmetrical-domain-security
source_filename: symmetrical-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symmetrical.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 11:42:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: symmetrical.ai\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symmetrical/refs/heads/main/security/symmetrical-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Payroll
- Human Resources
- Fintech
- Earned Wage Access
- Poland
---
