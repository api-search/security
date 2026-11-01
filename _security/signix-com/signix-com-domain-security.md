---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signix.com
  spf: true
hosts:
- host: signix.com
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Signix Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SIGNiX, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SIGNiX
provider_slug: signix-com
slug: signix-com-domain-security
source_filename: signix-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signix.com\n  https: false\ndomains:\n- domain: signix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/signix-com/security/signix-com-domain-security.yml
summary_line: DMARC
tags:
- Company
- DigitalSignature
- API
- Compliance
- RemoteNotarization
---
