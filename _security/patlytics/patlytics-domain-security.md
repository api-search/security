---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: patlytics.ai
  spf: true
hosts:
- cert_expires: Oct 15 21:34:25 2026 GMT
  host: www.patlytics.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 04:44:27 2026 GMT
  host: mcp.patlytics.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patlytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patlytics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Patlytics
provider_slug: patlytics
slug: patlytics-domain-security
source_filename: patlytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patlytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 21:34:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.patlytics.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 04:44:27 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: patlytics.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patlytics/refs/heads/main/security/patlytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Intellectual Property
- Patents
- Legal Tech
- Artificial Intelligence
- Patent Search
- Prior Art
- Model Context Protocol
- Agents
- Research
---
