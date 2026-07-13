---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: guildwars2.com
  spf: true
hosts:
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: wiki.guildwars2.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Guild Wars 2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guild Wars 2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Guild Wars 2
provider_slug: guild-wars-2
slug: guild-wars-2-domain-security
source_filename: guild-wars-2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wiki.guildwars2.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: guildwars2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guild-wars-2/refs/heads/main/security/guild-wars-2-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Games And Comics
- Public APIs
---
