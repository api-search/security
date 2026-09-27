---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ayima.com
  spf: true
hosts:
- cert_expires: Nov 18 08:08:07 2026 GMT
  host: www.ayima.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ayima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ayima, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ayima
provider_slug: ayima
slug: ayima-domain-security
source_filename: ayima-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ayima.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 08:08:07 2026 GMT\n  hsts: false\ndomains:\n- domain: ayima.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ayima/refs/heads/main/security/ayima-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SEO
- AI
- Marketing
- Consulting
- Enterprise
---
