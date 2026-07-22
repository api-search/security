---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aliciabots.com
  spf: true
hosts:
- cert_expires: Oct 13 19:46:38 2026 GMT
  host: aliciabots.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aliciabots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AliciaBots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AliciaBots
provider_slug: aliciabots
slug: aliciabots-domain-security
source_filename: aliciabots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aliciabots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 19:46:38 2026 GMT\n  hsts: false\ndomains:\n- domain: aliciabots.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aliciabots/refs/heads/main/security/aliciabots-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Robotics
- Maritime
- Autonomous Systems
- Hull Cleaning
- Shipping
- IoT
---
