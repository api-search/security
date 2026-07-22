---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: utopia.app
  spf: true
hosts:
- cert_expires: Sep 20 22:44:25 2026 GMT
  host: utopia.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utopia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utopia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Utopia
provider_slug: utopia
slug: utopia-domain-security
source_filename: utopia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utopia.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:44:25 2026 GMT\n  hsts: false\ndomains:\n- domain: utopia.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utopia/refs/heads/main/security/utopia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- Design
- Low Code
- React
- Open Source
---
