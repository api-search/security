---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evbox.com
  spf: true
hosts:
- cert_expires: Jan 22 10:10:59 2027 GMT
  host: evbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EVBox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EVBox
provider_slug: evbox
slug: evbox-domain-security
source_filename: evbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 10:10:59 2027 GMT\n  hsts: false\ndomains:\n- domain: evbox.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/evbox/security/evbox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- EVCharging
- Hardware
- Software
- Energy
---
