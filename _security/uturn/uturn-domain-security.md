---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uturn.me
  spf: true
hosts:
- cert_expires: Dec  1 10:26:18 2026 GMT
  host: uturn.me
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Uturn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UTURN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UTURN
provider_slug: uturn
slug: uturn-domain-security
source_filename: uturn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uturn.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  1 10:26:18 2026 GMT\n  hsts: false\ndomains:\n- domain: uturn.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uturn/refs/heads/main/security/uturn-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Media
- Entertainment
- Digital Content
- Multi-Channel Network
- Saudi Arabia
- MENA
---
