---
description: ''
domains:
- caa:
  - 0 issuewild "entrust.net"
  - 0 issuewild "sectigo.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  - 0 issuemail "sectigo.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parliament.uk
  spf: true
hosts:
- cert_expires: Oct  9 05:19:51 2026 GMT
  host: explore.data.parliament.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Parliament Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data.parliament.uk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Data.parliament.uk
provider_slug: data-parliament-uk
slug: data-parliament-uk-domain-security
source_filename: data-parliament-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: explore.data.parliament.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:19:51 2026 GMT\n  hsts: false\ndomains:\n- domain: parliament.uk\n  dnssec: false\n  caa:\n  - 0 issuewild \"entrust.net\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  - 0 issuemail \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-parliament-uk/refs/heads/main/security/data-parliament-uk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Government
- Public APIs
---
