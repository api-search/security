---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bkkstaff.com
  spf: true
hosts:
- cert_expires: Dec 27 14:44:27 2026 GMT
  host: bkkstaff.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bkkstaff Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BKK Staff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BKK Staff
provider_slug: bkkstaff-com
slug: bkkstaff-com-domain-security
source_filename: bkkstaff-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bkkstaff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 14:44:27 2026 GMT\n  hsts: false\ndomains:\n- domain: bkkstaff.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/bkkstaff-com/security/bkkstaff-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hiring
- Staffing
- Small Business
- Automation
- Thailand
---
