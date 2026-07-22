---
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: orolabs.ai
  spf: true
hosts:
- cert_expires: Sep 10 19:15:28 2026 GMT
  host: orolabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orolabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orolabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Orolabs
provider_slug: orolabs
slug: orolabs-domain-security
source_filename: orolabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orolabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:15:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orolabs.ai\n  dnssec: true\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orolabs/refs/heads/main/security/orolabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Procurement
- Spend Management
- Supplier Management
- Agentic AI
- Workflow Automation
- Enterprise Software
- ProcureTech
---
