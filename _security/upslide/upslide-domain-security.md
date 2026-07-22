---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: upslide.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: upslide.net
  spf: true
hosts:
- cert_expires: Oct 18 16:29:55 2026 GMT
  host: upslide.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: portal.upslide.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 23 23:41:01 2026 GMT
  host: support.upslide.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upslide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UpSlide, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: UpSlide
provider_slug: upslide
slug: upslide-domain-security
source_filename: upslide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upslide.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 16:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: portal.upslide.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.upslide.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:41:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: upslide.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: upslide.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upslide/refs/heads/main/security/upslide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Applicative Saas
- Document Automation
- Financial Services
- Microsoft 365
- PowerPoint
- Excel
- AI Assistants
- MCP
---
