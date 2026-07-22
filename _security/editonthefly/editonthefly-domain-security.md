---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: editonthefly.com
  spf: true
hosts:
- host: editonthefly.com
  https: false
kind: domain-security
layout: security
method: probed
name: Editonthefly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for editonthefly, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: editonthefly
provider_slug: editonthefly
slug: editonthefly-domain-security
source_filename: editonthefly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: editonthefly.com\n  https: false\ndomains:\n- domain: editonthefly.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/editonthefly/refs/heads/main/security/editonthefly-domain-security.yml
summary_line: DMARC
tags:
- Company
---
