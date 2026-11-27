---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mass.gov
  spf: true
hosts:
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: www.mass.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Commonwealth of Massachusetts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Commonwealth of Massachusetts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Commonwealth of Massachusetts
provider_slug: mass-gov
slug: mass-gov-domain-security
source_filename: mass-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mass.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: mass.gov\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mass-gov/security/mass-gov-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Massachusetts
- Public Data
- Open Data
---
