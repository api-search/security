---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workfusion.com
  spf: true
hosts:
- cert_expires: Oct 17 02:25:15 2026 GMT
  host: www.workfusion.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: doc.workfusion.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Workfusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorkFusion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WorkFusion
provider_slug: workfusion
slug: workfusion-domain-security
source_filename: workfusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:25:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: doc.workfusion.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: workfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workfusion/refs/heads/main/security/workfusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Financial Crime Compliance
- Anti-Money Laundering
- Sanctions Screening
- Know Your Customer
- Transaction Monitoring
- Adverse Media Monitoring
- Intelligent Document Processing
- Robotic Process Automation
- Banking
---
