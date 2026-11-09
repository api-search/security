---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: approval.studio
  spf: true
hosts:
- cert_expires: Dec 28 03:08:47 2026 GMT
  host: approval.studio
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Approval Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Approval Studio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Approval Studio
provider_slug: approval-studio
slug: approval-studio-domain-security
source_filename: approval-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: approval.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 03:08:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: approval.studio\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/approval-studio/security/approval-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artwork
- Design
- Approval
- Collaboration
- Artificial Intelligence
---
