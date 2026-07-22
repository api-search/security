---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: billables.ai
  spf: true
hosts:
- cert_expires: Oct 15 18:39:57 2026 GMT
  host: billables.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Billables Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billables Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Billables Ai
provider_slug: billables-ai
slug: billables-ai-domain-security
source_filename: billables-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billables.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 18:39:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billables.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billables-ai/refs/heads/main/security/billables-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Tech
- Time Tracking
- Timekeeping
- Billing
- Artificial Intelligence
- Professional Services
- Productivity
---
