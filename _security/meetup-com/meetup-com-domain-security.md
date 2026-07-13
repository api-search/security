---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
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
kind: domain-security
layout: security
method: probed
name: Meetup Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meetup.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meetup.com
provider_slug: meetup-com
slug: meetup-com-domain-security
source_filename: meetup-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetup.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  6 19:03:05 2027 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: meetup.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meetup-com/refs/heads/main/security/meetup-com-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Social
- Public APIs
---
