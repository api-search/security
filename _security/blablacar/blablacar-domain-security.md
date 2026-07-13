---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blablacar.com
  spf: true
hosts:
- cert_expires: Aug  3 14:30:19 2026 GMT
  host: dev.blablacar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blablacar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlaBlaCar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BlaBlaCar
provider_slug: blablacar
slug: blablacar-domain-security
source_filename: blablacar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.blablacar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  3 14:30:19 2026 GMT\n  hsts: null\ndomains:\n- domain: blablacar.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blablacar/refs/heads/main/security/blablacar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
