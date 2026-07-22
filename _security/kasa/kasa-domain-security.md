---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kasa.com
  spf: true
hosts:
- cert_expires: Aug 29 16:23:49 2026 GMT
  host: kasa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kasa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kasa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kasa
provider_slug: kasa
slug: kasa-domain-security
source_filename: kasa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:23:49 2026 GMT\n  hsts: null\ndomains:\n- domain: kasa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kasa/refs/heads/main/security/kasa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Proptech
- Hospitality
- Travel
- Lodging
- Short-Term Rental
- Corporate Housing
- Real Estate
---
