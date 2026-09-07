---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oneaix.com
  spf: true
hosts:
- cert_expires: Jan 24 05:56:33 2027 GMT
  host: www.oneaix.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 1Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ONEAIX (1data / Yida Technology), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ONEAIX (1data / Yida Technology)
provider_slug: 1data
slug: 1data-domain-security
source_filename: 1data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oneaix.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 05:56:33 2027 GMT\n  hsts: false\ndomains:\n- domain: oneaix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1data/refs/heads/main/security/1data-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Large Language Models
- Supply Chain
- Logistics
- Freight Forwarding
- Robotic Process Automation
- Digital Workers
- Enterprise Software
- E-Commerce
- China
---
