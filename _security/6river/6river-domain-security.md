---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 6river.com
  spf: true
hosts:
- cert_expires: Jan 19 18:42:23 2027 GMT
  host: 6river.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6River Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6river, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 6river
provider_slug: 6river
slug: 6river-domain-security
source_filename: 6river-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 6river.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 18:42:23 2027 GMT\n  hsts: false\ndomains:\n- domain: 6river.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6river/refs/heads/main/security/6river-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Warehouse Automation
- Robotics
- Autonomous Mobile Robots
- Fulfillment
- Logistics
- Supply Chain
- Warehouse Management
---
