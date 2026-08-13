---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: fusewp.com
  spf: true
hosts:
- cert_expires: Oct 14 21:58:16 2026 GMT
  host: fusewp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 21:58:16 2026 GMT
  host: auth.fusewp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fusewp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FuseWP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FuseWP
provider_slug: fusewp
slug: fusewp-domain-security
source_filename: fusewp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fusewp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:58:16 2026 GMT\n  hsts: false\n- host: auth.fusewp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 21:58:16 2026 GMT\n  hsts: false\ndomains:\n- domain: fusewp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusewp/refs/heads/main/security/fusewp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- WordPress
- Email Marketing
- Marketing Automation
- CRM
- Integration
- Data Synchronization
- OAuth
- Plugins
- No Code
---
