---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: talkiatry.com
  spf: true
hosts:
- cert_expires: Oct 14 15:04:46 2026 GMT
  host: www.talkiatry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkiatry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkiatry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Talkiatry
provider_slug: talkiatry
slug: talkiatry-domain-security
source_filename: talkiatry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkiatry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 15:04:46 2026 GMT\n  hsts: false\ndomains:\n- domain: talkiatry.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkiatry/refs/heads/main/security/talkiatry-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Mental Health
- Telehealth
- Telepsychiatry
- Psychiatry
- Behavioral Health
- Digital Health
---
