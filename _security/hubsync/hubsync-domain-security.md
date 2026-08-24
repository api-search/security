---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hubsync.com
  spf: true
hosts:
- cert_expires: Oct  9 20:59:27 2026 GMT
  host: hubsync.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hubsync Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HubSync, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: HubSync
provider_slug: hubsync
slug: hubsync-domain-security
source_filename: hubsync-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubsync.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 20:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hubsync.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hubsync/refs/heads/main/security/hubsync-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tax
- Accounting
- Workflow Automation
- Document Management
- Electronic Signature
- Professional Services
- Artificial Intelligence
- Model Context Protocol
- SaaS
---
