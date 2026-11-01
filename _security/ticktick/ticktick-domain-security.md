---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ticktick.com
  spf: true
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: ticktick.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ticktick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TickTick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TickTick
provider_slug: ticktick
slug: ticktick-domain-security
source_filename: ticktick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ticktick.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ticktick.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ticktick/security/ticktick-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Productivity
- Task Management
- Calendar
- Collaboration
---
