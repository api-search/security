---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: playvs.com
  spf: true
hosts:
- cert_expires: Sep 26 14:12:15 2026 GMT
  host: playvs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Play Versus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Play Versus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Play Versus
provider_slug: play-versus
slug: play-versus-domain-security
source_filename: play-versus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playvs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:12:15 2026 GMT\n  hsts: false\ndomains:\n- domain: playvs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/play-versus/refs/heads/main/security/play-versus-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Esports
- Gaming
- Education
- Scholastic
- Competitions
- EdTech
---
