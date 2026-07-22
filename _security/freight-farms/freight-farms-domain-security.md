---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freightfarms.com
  spf: true
hosts:
- cert_expires: Oct  6 07:16:12 2026 GMT
  host: freightfarms.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freight Farms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freight Farms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freight Farms
provider_slug: freight-farms
slug: freight-farms-domain-security
source_filename: freight-farms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freightfarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:16:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: freightfarms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freight-farms/refs/heads/main/security/freight-farms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Farming
- Agriculture
- AgTech
- Hydroponics
- Controlled Environment Agriculture
- Container Farming
- Farm Automation
- IoT
- Food Technology
---
