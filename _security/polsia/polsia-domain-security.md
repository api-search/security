---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polsia.com
  spf: true
hosts:
- cert_expires: Sep 30 07:55:44 2026 GMT
  host: polsia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polsia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polsia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Polsia
provider_slug: polsia
slug: polsia-domain-security
source_filename: polsia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polsia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:55:44 2026 GMT\n  hsts: false\ndomains:\n- domain: polsia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polsia/refs/heads/main/security/polsia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Software
- Artificial Intelligence
- AI Agents
- Automation
- Business Automation
- SaaS
- Autonomous Agents
---
