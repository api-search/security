---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hyvor.com
  spf: true
hosts:
- cert_expires: Dec 10 06:46:32 2026 GMT
  host: hyvor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hyvor Talk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hyvor Talk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hyvor Talk
provider_slug: hyvor-talk
slug: hyvor-talk-domain-security
source_filename: hyvor-talk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hyvor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:46:32 2026 GMT\n  hsts: false\ndomains:\n- domain: hyvor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hyvor-talk/security/hyvor-talk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- comments
- platform
- SaaS
- engagement
- privacy
---
