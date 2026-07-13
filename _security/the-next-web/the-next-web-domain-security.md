---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "certainly.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thenextweb.com
  spf: true
hosts:
- cert_expires: Aug 30 19:48:41 2026 GMT
  host: thenextweb.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Next Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Next Web, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: The Next Web
provider_slug: the-next-web
slug: the-next-web-domain-security
source_filename: the-next-web-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thenextweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:48:41 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: thenextweb.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-next-web/refs/heads/main/security/the-next-web-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology News
- Innovation
- Media
- Events
- Startups
- Artificial Intelligence
---
