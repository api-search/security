---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "trust-provider.com"
  - 0 issuewild "usertrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cbs.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: www.cbs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cbs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CBS (Paramount Global), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CBS (Paramount Global)
provider_slug: cbs
slug: cbs-domain-security
source_filename: cbs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cbs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cbs.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"trust-provider.com\"\n  - 0 issuewild \"usertrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cbs/refs/heads/main/security/cbs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Broadcasting
- CBS News
- CBS Sports
- Entertainment
- Media
- News
- Paramount
- Streaming
- Television
- Fortune 500
---
