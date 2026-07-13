---
description: ''
domains:
- caa:
  - nat236919.github.io.
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: true
  domain: nuttaphat.com
  spf: false
hosts:
- cert_expires: Sep 28 08:14:24 2026 GMT
  host: nuttaphat.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covid 19 Jhu Csse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covid-19 JHU CSSE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Covid-19 JHU CSSE
provider_slug: covid-19-jhu-csse
slug: covid-19-jhu-csse-domain-security
source_filename: covid-19-jhu-csse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuttaphat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 08:14:24 2026 GMT\n  hsts: false\ndomains:\n- domain: nuttaphat.com\n  dnssec: true\n  caa:\n  - nat236919.github.io.\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covid-19-jhu-csse/refs/heads/main/security/covid-19-jhu-csse-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Health
- Public APIs
---
