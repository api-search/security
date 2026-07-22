---
description: ''
domains:
- caa:
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liazon.com
  spf: true
hosts:
- host: liazon.com
  https: false
kind: domain-security
layout: security
method: probed
name: Liazon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liazon, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Liazon
provider_slug: liazon
slug: liazon-domain-security
source_filename: liazon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liazon.com\n  https: false\ndomains:\n- domain: liazon.com\n  dnssec: false\n  caa:\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liazon/refs/heads/main/security/liazon-domain-security.yml
summary_line: DMARC
tags:
- Company
- Commerce
- Employee Benefits
- Insurance
- Health Insurance
- Benefits Administration
- Private Benefits Exchange
- Acquired
- WTW
---
