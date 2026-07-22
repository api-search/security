---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: stopbreathethink.com
  spf: false
hosts:
- host: stopbreathethink.com
  https: false
kind: domain-security
layout: security
method: probed
name: Mylife Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyLife, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MyLife
provider_slug: mylife
slug: mylife-domain-security
source_filename: mylife-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stopbreathethink.com\n  https: false\ndomains:\n- domain: stopbreathethink.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mylife/refs/heads/main/security/mylife-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Meditation
- Mindfulness
- Wellness
- Mental Health
- Mobile App
- Consumer
---
