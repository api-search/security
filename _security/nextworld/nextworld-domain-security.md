---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nextw.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nextworld.net
  spf: true
hosts:
- cert_expires: Oct 17 09:39:53 2026 GMT
  host: www.nextw.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: apps.nextworld.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nextworld Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nextworld, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nextworld
provider_slug: nextworld
slug: nextworld-domain-security
source_filename: nextworld-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 09:39:53 2026 GMT\n  hsts: false\n- host: apps.nextworld.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nextw.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nextworld.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextworld/refs/heads/main/security/nextworld-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Enterprise Resource Planning
- No-Code
- Enterprise Application Platform
- Workflow Automation
- Artificial Intelligence
- Model Context Protocol
- Integration
- Manufacturing
- Distribution
---
