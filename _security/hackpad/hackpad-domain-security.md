---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  dmarc: false
  dnssec: false
  domain: hackpad.com
  spf: true
hosts:
- host: hackpad.com
  https: false
kind: domain-security
layout: security
method: probed
name: Hackpad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hackpad, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hackpad
provider_slug: hackpad
slug: hackpad-domain-security
source_filename: hackpad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hackpad.com\n  https: false\ndomains:\n- domain: hackpad.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hackpad/refs/heads/main/security/hackpad-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Collaboration
- Documents
- Wiki
- Real-Time Editing
- Productivity
- Open Source
---
