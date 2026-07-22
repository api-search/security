---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anglers.jp
  spf: true
hosts:
- cert_expires: Oct  6 02:24:08 2026 GMT
  host: anglers.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anglers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anglers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anglers
provider_slug: anglers
slug: anglers-domain-security
source_filename: anglers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anglers.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 02:24:08 2026 GMT\n  hsts: false\ndomains:\n- domain: anglers.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anglers/refs/heads/main/security/anglers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
