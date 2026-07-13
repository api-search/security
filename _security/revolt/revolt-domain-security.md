---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revolt.chat
  spf: true
hosts:
- cert_expires: Aug 24 19:44:38 2026 GMT
  host: developers.revolt.chat
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revolt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revolt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revolt
provider_slug: revolt
slug: revolt-domain-security
source_filename: revolt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.revolt.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:44:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: revolt.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolt/refs/heads/main/security/revolt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social
- Public APIs
---
