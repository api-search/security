---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mcmakler.de
  spf: true
hosts:
- cert_expires: Sep 29 11:00:50 2026 GMT
  host: www.mcmakler.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mcmakler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcmakler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: mcmakler
provider_slug: mcmakler
slug: mcmakler-domain-security
source_filename: mcmakler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mcmakler.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:00:50 2026 GMT\n  hsts: false\ndomains:\n- domain: mcmakler.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcmakler/refs/heads/main/security/mcmakler-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- Proptech
- Germany
- Brokerage
- Housing
---
