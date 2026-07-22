---
description: ''
domains:
- caa:
  - 0 iodef "\"mailto:sysadmin@subway.com\""
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "sectigo.com"
  - 0 issue "godaddy.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: subway.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.subway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Subway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Subway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Subway
provider_slug: subway
slug: subway-domain-security
source_filename: subway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.subway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: subway.com\n  dnssec: false\n  caa:\n  - 0 iodef \"\\\"mailto:sysadmin@subway.com\\\"\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/subway/refs/heads/main/security/subway-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fast Food
- Restaurants
- Food & Beverage
- Quick Service Restaurant
- Loyalty
---
