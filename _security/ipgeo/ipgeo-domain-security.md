---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: techniknews.net
  spf: true
hosts:
- cert_expires: Aug 26 17:46:12 2026 GMT
  host: api.techniknews.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipgeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPGEO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IPGEO
provider_slug: ipgeo
slug: ipgeo-domain-security
source_filename: ipgeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.techniknews.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 17:46:12 2026 GMT\n  hsts: false\ndomains:\n- domain: techniknews.net\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipgeo/refs/heads/main/security/ipgeo-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Geocoding
- Public APIs
---
