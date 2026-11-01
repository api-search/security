---
description: ''
domains:
- caa:
  - 0 issue ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cuspai.com
  spf: true
hosts:
- host: www.cuspai.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuspai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuspai, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cuspai
provider_slug: cuspai-com
slug: cuspai-com-domain-security
source_filename: cuspai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cuspai.com\n  https: false\ndomains:\n- domain: cuspai.com\n  dnssec: true\n  caa:\n  - 0 issue \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cuspai-com/security/cuspai-com-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- AI
- Data-Analytics
- Automation
- Cloud
---
