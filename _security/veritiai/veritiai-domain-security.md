---
description: ''
domains:
- caa:
  - d396y8eo3tk9fl.cloudfront.net.
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: veriti.ai
  spf: false
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: veriti.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veritiai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veriti.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Veriti.ai
provider_slug: veritiai
slug: veritiai-domain-security
source_filename: veritiai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veriti.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: veriti.ai\n  dnssec: true\n  caa:\n  - d396y8eo3tk9fl.cloudfront.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritiai/refs/heads/main/security/veritiai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Exposure Management
- Vulnerability Management
- Threat Intelligence
- Remediation
- Security Automation
---
