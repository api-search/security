---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild ";"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: obsproject.com
  spf: true
hosts:
- cert_expires: Dec 27 05:50:20 2026 GMT
  host: obsproject.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OBS Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OBS Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OBS Studio
provider_slug: obs-studio
slug: obs-studio-domain-security
source_filename: obs-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: obsproject.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 05:50:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: obsproject.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \";\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/obs-studio/security/obs-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Video Recording
- Live Streaming
- Open-source software
---
