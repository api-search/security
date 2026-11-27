---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: tenjin.sh
  spf: true
hosts:
- cert_expires: Feb 19 22:25:00 2027 GMT
  host: tenjin.sh
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tenjin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tenjin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tenjin
provider_slug: tenjin-sh
slug: tenjin-sh-domain-security
source_filename: tenjin-sh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tenjin.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 22:25:00 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tenjin.sh\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/tenjin-sh/security/tenjin-sh-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Tooling
- Automation
- Agent
- Platform
---
