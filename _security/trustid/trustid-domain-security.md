---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trustid.com
  spf: true
hosts:
- host: trustid.com
  https: false
kind: domain-security
layout: security
method: probed
name: Trustid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trustid, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trustid
provider_slug: trustid
slug: trustid-domain-security
source_filename: trustid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trustid.com\n  https: false\ndomains:\n- domain: trustid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustid/refs/heads/main/security/trustid-domain-security.yml
summary_line: DMARC
tags:
- Company
- Caller Authentication
- Identity
- Fraud Prevention
- Call Centers
- Telecommunications
- Acquired
---
