---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ip2whois.com
  spf: false
hosts:
- cert_expires: Oct  8 00:23:25 2026 GMT
  host: www.ip2whois.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ip2Whois Information Lookup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IP2WHOIS Information Lookup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: IP2WHOIS Information Lookup
provider_slug: ip2whois-information-lookup
slug: ip2whois-information-lookup-domain-security
source_filename: ip2whois-information-lookup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ip2whois.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 00:23:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ip2whois.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ip2whois-information-lookup/refs/heads/main/security/ip2whois-information-lookup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Development
- Public APIs
---
