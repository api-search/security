---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: layrcake.dev
  spf: true
hosts:
- cert_expires: Dec 14 01:21:17 2026 GMT
  host: layrcake.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Layrcake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layrcake, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Layrcake
provider_slug: layrcake-dev
slug: layrcake-dev-domain-security
source_filename: layrcake-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layrcake.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 01:21:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: layrcake.dev\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/layrcake-dev/security/layrcake-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Marketing
- Outreach
- Automation
- Software-as-a-Service
---
