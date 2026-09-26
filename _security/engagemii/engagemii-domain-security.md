---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: engagemii.com
  spf: true
hosts:
- cert_expires: Dec 10 03:40:09 2026 GMT
  host: engagemii.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Engagemii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engagemii Citation Watch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Engagemii Citation Watch
provider_slug: engagemii
slug: engagemii-domain-security
source_filename: engagemii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: engagemii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 03:40:09 2026 GMT\n  hsts: false\ndomains:\n- domain: engagemii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagemii/refs/heads/main/security/engagemii-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Visibility
- Analytics
- Free
---
