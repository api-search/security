---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zoca.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: zoca.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zoca
provider_slug: zoca
slug: zoca-domain-security
source_filename: zoca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zoca.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zoca.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoca/refs/heads/main/security/zoca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Marketing
- Beauty and Wellness
- Local Business
- AI Agents
- Appointments
- SaaS
---
