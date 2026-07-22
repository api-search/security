---
description: ''
domains:
- caa:
  - 6a1c46976feeb78656562f1cf0923fb4.qcloudwzgj.com.
  - 4bf15620b49cf7f1-cl2.qcloudcjgj.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: roxmotor.com
  spf: true
hosts:
- host: roxmotor.com
  https: false
kind: domain-security
layout: security
method: probed
name: Roxmotor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for roxmotor, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: roxmotor
provider_slug: roxmotor
slug: roxmotor-domain-security
source_filename: roxmotor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: roxmotor.com\n  https: false\ndomains:\n- domain: roxmotor.com\n  dnssec: true\n  caa:\n  - 6a1c46976feeb78656562f1cf0923fb4.qcloudwzgj.com.\n  - 4bf15620b49cf7f1-cl2.qcloudcjgj.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roxmotor/refs/heads/main/security/roxmotor-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Automotive
- Electric Vehicles
- Mobility
- China
- Startup
---
