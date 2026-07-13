---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meetup.com
  spf: true
hosts:
- cert_expires: Mar  6 19:03:05 2027 GMT
  host: www.meetup.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  6 19:03:05 2027 GMT
  host: api.meetup.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Meetup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meetup, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meetup
provider_slug: meetup
slug: meetup-domain-security
source_filename: meetup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 19:03:05 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: api.meetup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 19:03:05 2027 GMT\n  hsts: null\ndomains:\n- domain: meetup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meetup/refs/heads/main/security/meetup-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Events
- Community
- Groups
- Meetups
- Social
- GraphQL
---
