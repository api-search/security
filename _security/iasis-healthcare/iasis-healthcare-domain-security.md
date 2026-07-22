---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: steward.org
  spf: true
hosts:
- host: www.steward.org
  https: false
kind: domain-security
layout: security
method: probed
name: Iasis Healthcare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IASIS Healthcare, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IASIS Healthcare
provider_slug: iasis-healthcare
slug: iasis-healthcare-domain-security
source_filename: iasis-healthcare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.steward.org\n  https: false\ndomains:\n- domain: steward.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iasis-healthcare/refs/heads/main/security/iasis-healthcare-domain-security.yml
summary_line: DMARC
tags:
- Acquired
- Healthcare
- Hospitals
- Legacy
---
