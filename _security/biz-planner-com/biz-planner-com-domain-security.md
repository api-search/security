---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biz-planner.com
  spf: false
hosts:
- cert_expires: Jan 28 13:56:45 2027 GMT
  host: biz-planner.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BizPlanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BizPlanner, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: BizPlanner
provider_slug: biz-planner-com
slug: biz-planner-com-domain-security
source_filename: biz-planner-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biz-planner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 13:56:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biz-planner.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/biz-planner-com/security/biz-planner-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Artificial Intelligence
- Simulation
- Entrepreneurship
- Software-as-a-Service
---
