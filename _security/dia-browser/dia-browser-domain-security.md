---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: diabrowser.com
  spf: true
hosts:
- cert_expires: Sep 13 16:48:19 2026 GMT
  host: www.diabrowser.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dia Browser Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dia (The Browser Company), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dia (The Browser Company)
provider_slug: dia-browser
slug: dia-browser-domain-security
source_filename: dia-browser-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diabrowser.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: diabrowser.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dia-browser/refs/heads/main/security/dia-browser-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser
- AI Browser
- Agent
- Consumer
- The Browser Company
---
