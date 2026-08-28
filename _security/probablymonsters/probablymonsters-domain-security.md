---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: probablymonsters.com
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: www.probablymonsters.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Probablymonsters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProbablyMonsters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ProbablyMonsters
provider_slug: probablymonsters
slug: probablymonsters-domain-security
source_filename: probablymonsters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.probablymonsters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: probablymonsters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/probablymonsters/refs/heads/main/security/probablymonsters-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Video Games
- Game Development
- Game Studios
- Interactive Entertainment
- Entertainment
- Media
---
