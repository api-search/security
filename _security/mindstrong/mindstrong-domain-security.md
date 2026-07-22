---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mindstrong.com
  spf: true
hosts:
- host: mindstrong.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mindstrong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindstrong, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mindstrong
provider_slug: mindstrong
slug: mindstrong-domain-security
source_filename: mindstrong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindstrong.com\n  https: false\ndomains:\n- domain: mindstrong.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindstrong/refs/heads/main/security/mindstrong-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Mental Health
- Digital Health
- Behavioral Health
- Digital Biomarkers
- Health Technology
---
