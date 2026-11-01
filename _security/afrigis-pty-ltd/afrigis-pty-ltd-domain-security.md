---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: afrigis.co.za
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: www.afrigis.co.za
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afrigis Pty Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AfriGIS (Pty) Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: AfriGIS (Pty) Ltd
provider_slug: afrigis-pty-ltd
slug: afrigis-pty-ltd-domain-security
source_filename: afrigis-pty-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.afrigis.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: afrigis.co.za\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/afrigis-pty-ltd/security/afrigis-pty-ltd-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
