---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: chargezoom.com
  spf: true
hosts:
- cert_expires: Dec 29 04:19:10 2026 GMT
  host: www.chargezoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chargezoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chargezoom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Chargezoom
provider_slug: chargezoom
slug: chargezoom-domain-security
source_filename: chargezoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chargezoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 04:19:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: chargezoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chargezoom/refs/heads/main/security/chargezoom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- Payments
- Automation
- AI
---
