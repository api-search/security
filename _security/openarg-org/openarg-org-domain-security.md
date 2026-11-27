---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: false
  dnssec: false
  domain: openarg.org
  spf: false
hosts:
- cert_expires: Feb 14 10:26:14 2027 GMT
  host: openarg.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenArg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenArg, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenArg
provider_slug: openarg-org
slug: openarg-org-domain-security
source_filename: openarg-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openarg.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 10:26:14 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openarg.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openarg-org/security/openarg-org-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data
- Artificial Intelligence
- Open Data
- Argentina
- PublicDatasets
---
