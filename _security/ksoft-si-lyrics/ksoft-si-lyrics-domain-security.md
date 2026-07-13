---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: ksoft.si
  spf: true
hosts:
- host: docs.ksoft.si
  https: false
kind: domain-security
layout: security
method: probed
name: Ksoft Si Lyrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KSoft.Si Lyrics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: KSoft.Si Lyrics
provider_slug: ksoft-si-lyrics
slug: ksoft-si-lyrics-domain-security
source_filename: ksoft-si-lyrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ksoft.si\n  https: false\ndomains:\n- domain: ksoft.si\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ksoft-si-lyrics/refs/heads/main/security/ksoft-si-lyrics-domain-security.yml
summary_line: DNSSEC
tags:
- Music
- Public APIs
---
