---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: honeyhomes.com
  spf: true
hosts:
- cert_expires: Oct 14 06:12:55 2026 GMT
  host: www.honeyhomes.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Honeyhomes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honeyhomes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Honeyhomes
provider_slug: honeyhomes
slug: honeyhomes-domain-security
source_filename: honeyhomes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honeyhomes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:12:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: honeyhomes.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeyhomes/refs/heads/main/security/honeyhomes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Home Services
- Home Maintenance
- Handyman
- Property Management
- Membership
- Consumer Services
- Real Estate
---
