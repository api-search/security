---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nytimes.com
  spf: true
hosts:
- cert_expires: Aug 20 03:39:39 2026 GMT
  host: developer.nytimes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: New York Times Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for New York Times, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: New York Times
provider_slug: new-york-times
slug: new-york-times-domain-security
source_filename: new-york-times-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nytimes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 03:39:39 2026 GMT\n  hsts: null\ndomains:\n- domain: nytimes.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-times/refs/heads/main/security/new-york-times-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- News
- Public APIs
---
