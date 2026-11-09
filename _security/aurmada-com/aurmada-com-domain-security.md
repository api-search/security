---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aurmada.com
  spf: true
hosts:
- cert_expires: Dec 10 13:04:37 2026 GMT
  host: aurmada.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurmada Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurmada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aurmada
provider_slug: aurmada-com
slug: aurmada-com-domain-security
source_filename: aurmada-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurmada.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 13:04:37 2026 GMT\n  hsts: null\ndomains:\n- domain: aurmada.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aurmada-com/security/aurmada-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Robotics
- Platform
- Os
- Human-Computer Interaction
---
