---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: theladders.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: theladders.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: The Ladders Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Ladders, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Ladders
provider_slug: the-ladders
slug: the-ladders-domain-security
source_filename: the-ladders-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theladders.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: theladders.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-ladders/refs/heads/main/security/the-ladders-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Consumer
- Jobs
- Careers
- Recruiting
- Job Search
- Executive Jobs
- Employment
- HR Tech
---
