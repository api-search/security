---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anoram.com
  spf: true
hosts:
- cert_expires: Aug 29 15:34:12 2026 GMT
  host: biriyani.anoram.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biriyani As A Service Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biriyani As A Service, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biriyani As A Service
provider_slug: biriyani-as-a-service
slug: biriyani-as-a-service-domain-security
source_filename: biriyani-as-a-service-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biriyani.anoram.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:34:12 2026 GMT\n  hsts: null\ndomains:\n- domain: anoram.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biriyani-as-a-service/refs/heads/main/security/biriyani-as-a-service-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Personality
- Public APIs
---
