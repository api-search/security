---
description: ''
domains:
- caa:
  - sma-web-alb-483011900.eu-central-1.elb.amazonaws.com.
  dmarc: false
  dnssec: true
  domain: zeversolar.com
  spf: false
hosts:
- cert_expires: May 26 00:39:37 2027 GMT
  host: zeversolar.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zevercloud (Zeversolar) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zevercloud (Zeversolar), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Zevercloud (Zeversolar)
provider_slug: zeversolar
slug: zeversolar-domain-security
source_filename: zeversolar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeversolar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 26 00:39:37 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: zeversolar.com\n  dnssec: true\n  caa:\n  - sma-web-alb-483011900.eu-central-1.elb.amazonaws.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/zeversolar/security/zeversolar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Solar
- Energy
- Germany
- Ceased-Operations
---
