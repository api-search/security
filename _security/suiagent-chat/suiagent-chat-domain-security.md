---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: suiagent.chat
  spf: true
hosts:
- host: suiagent.chat
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: suiagent-chat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for suiagent-chat, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: suiagent-chat
provider_slug: suiagent-chat
slug: suiagent-chat-domain-security
source_filename: suiagent-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: suiagent.chat\n  https: false\ndomains:\n- domain: suiagent.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/suiagent-chat/security/suiagent-chat-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
