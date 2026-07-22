---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinpaladin.com
  spf: true
hosts:
- cert_expires: Oct 16 00:23:06 2026 GMT
  host: joinpaladin.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paladin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paladin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Paladin
provider_slug: paladin
slug: paladin-domain-security
source_filename: paladin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinpaladin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:23:06 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: joinpaladin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paladin/refs/heads/main/security/paladin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Technology
- Pro Bono
- Legal Services
- Volunteer Management
- Program Management
- Compliance
---
