---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clingsystems.com
  spf: true
hosts:
- cert_expires: Jan  6 07:00:52 2027 GMT
  host: clingsystems.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clingsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clingsystems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clingsystems
provider_slug: clingsystems
slug: clingsystems-domain-security
source_filename: clingsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clingsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 07:00:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clingsystems.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clingsystems/refs/heads/main/security/clingsystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Battery
- Marketplace
- circular-economy
- Sustainability
- Sweden
---
