---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: talentanvil.com
  spf: true
hosts:
- cert_expires: Jan 24 08:45:41 2027 GMT
  host: talentanvil.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TalentAnvil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TalentAnvil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TalentAnvil
provider_slug: talentanvil-com
slug: talentanvil-com-domain-security
source_filename: talentanvil-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: talentanvil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 08:45:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: talentanvil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/talentanvil-com/security/talentanvil-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gaming
- World of Warcraft
- Talent Calculator
- AI
- Free Tool
---
