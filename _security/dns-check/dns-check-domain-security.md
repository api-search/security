---
api_specs:
- filename: dns-check-openapi.yml
  format: yaml
  label: DNS Check REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dns-check/refs/heads/main/openapi/dns-check-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dnscheck.co
  spf: true
hosts:
- cert_expires: Aug 17 17:36:38 2026 GMT
  host: www.dnscheck.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dns Check Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNS Check, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DNS Check
provider_slug: dns-check
slug: dns-check-domain-security
source_filename: dns-check-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dnscheck.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:36:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dnscheck.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dns-check/refs/heads/main/security/dns-check-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS
- DNS Monitoring
- Domain Monitoring
- DNS Records
- Infrastructure Monitoring
- Networking
---
