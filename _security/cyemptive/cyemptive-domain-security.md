---
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cyemptive.com
  spf: true
hosts:
- host: www.cyemptive.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cyemptive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cyemptive, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cyemptive
provider_slug: cyemptive
slug: cyemptive-domain-security
source_filename: cyemptive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cyemptive.com\n  https: false\ndomains:\n- domain: cyemptive.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cyemptive/refs/heads/main/security/cyemptive-domain-security.yml
summary_line: DMARC
tags:
- Company
- Cybersecurity
- Security
- Ransomware
- Endpoint Security
- Cloud Security
- Threat Prevention
- Zero Trust
- Compliance
- Government
---
