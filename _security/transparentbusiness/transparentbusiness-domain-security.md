---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: transparentbusiness.com
  spf: true
hosts:
- cert_expires: Nov  3 09:13:16 2026 GMT
  host: transparentbusiness.com
  hsts: max-age=2592000; includeSubDomains; preload
  http_status: 403
  https: true
  note: The origin is fronted by Cloudflare and answers every automated request with a 403 "Attention Required!" interstitial; the HSTS header above was read off that 403 response, which is why the automated probe recorded it as absent.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transparentbusiness Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TransparentBusiness, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TransparentBusiness
provider_slug: transparentbusiness
slug: transparentbusiness-domain-security
source_filename: transparentbusiness-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transparentbusiness.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  3 09:13:16 2026 GMT\n  hsts: max-age=2592000; includeSubDomains; preload\n  http_status: 403\n  note: 'The origin is fronted by Cloudflare and answers every automated request with a 403 \"Attention\n    Required!\" interstitial; the HSTS header above was read off that 403 response, which is why the\n    automated probe recorded it as absent.'\ndomains:\n- domain: transparentbusiness.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transparentbusiness/refs/heads/main/security/transparentbusiness-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Remote Work
- Workforce Management
- Time Tracking
- Productivity
- Project Management
- Human Resources
- SaaS
---
