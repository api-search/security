---
description: ''
domains:
- caa:
  - 0 iodef "mailto:contact_pki@apple.com"
  - 0 issue "pki.apple.com"
  - 0 issuewild "pki.apple.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apple.com
  spf: true
hosts:
- host: affiliate.itunes.apple.com
  https: false
kind: domain-security
layout: security
method: probed
name: Itunes Search Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iTunes Search, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iTunes Search
provider_slug: itunes-search
slug: itunes-search-domain-security
source_filename: itunes-search-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: affiliate.itunes.apple.com\n  https: false\ndomains:\n- domain: apple.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:contact_pki@apple.com\"\n  - 0 issue \"pki.apple.com\"\n  - 0 issuewild \"pki.apple.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itunes-search/refs/heads/main/security/itunes-search-domain-security.yml
summary_line: DMARC
tags:
- Music
- Public APIs
---
