---
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cutover.com
  spf: true
hosts:
- cert_expires: Sep 17 01:46:00 2026 GMT
  host: cutover.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:40:02 2026 GMT
  host: developer.cutover.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.cutover.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cutover Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cutover, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cutover
provider_slug: cutover
slug: cutover-domain-security
source_filename: cutover-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cutover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 01:46:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.cutover.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:40:02 2026 GMT\n  hsts: false\n- host: api.cutover.com\n  https: false\ndomains:\n- domain: cutover.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutover/refs/heads/main/security/cutover-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- IT Operations
- Disaster Recovery
- Incident Management
- Runbook Automation
- Orchestration
- Workflow Automation
- DevOps
---
