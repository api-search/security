---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: approve.com
  spf: true
hosts:
- host: approve.com
  https: false
kind: domain-security
layout: security
method: probed
name: Approvecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Approve.com, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Approve.com
provider_slug: approvecom
slug: approvecom-domain-security
source_filename: approvecom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: approve.com\n  https: false\ndomains:\n- domain: approve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/approvecom/refs/heads/main/security/approvecom-domain-security.yml
summary_line: DMARC
tags:
- Company
- Procurement
- Purchase Orders
- Spend Management
- Accounts Payable
- Vendor Management
- Finance
- Approvals
- B2B
---
