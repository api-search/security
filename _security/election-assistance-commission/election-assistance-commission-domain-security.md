---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eac.gov
  spf: true
hosts:
- cert_expires: Sep  8 20:47:38 2026 GMT
  host: www.eac.gov
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Election Assistance Commission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Election Assistance Commission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Election Assistance Commission
provider_slug: election-assistance-commission
slug: election-assistance-commission-domain-security
source_filename: election-assistance-commission-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eac.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:47:38 2026 GMT\n  hsts: false\ndomains:\n- domain: eac.gov\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/election-assistance-commission/refs/heads/main/security/election-assistance-commission-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Federal Government
- Elections
- Voting
- Open Data
---
