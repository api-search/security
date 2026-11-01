---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tencent.com
  spf: true
hosts:
- host: tencent.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tencent Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tencent, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tencent
provider_slug: tencent-com
slug: tencent-com-domain-security
source_filename: tencent-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tencent.com\n  https: false\ndomains:\n- domain: tencent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tencent-com/security/tencent-com-domain-security.yml
summary_line: DMARC
tags:
- Company
---
