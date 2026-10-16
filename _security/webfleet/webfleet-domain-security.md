---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: webfleet.com
  spf: true
hosts:
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: www.webfleet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Webfleet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webfleet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Webfleet
provider_slug: webfleet
slug: webfleet-domain-security
source_filename: webfleet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.webfleet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: webfleet.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webfleet/refs/heads/main/security/webfleet-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fleet Management
- GPS Tracking
- Vehicle Telematics
- Logistics
---
