---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dhsdigital.eu
  spf: true
hosts:
- cert_expires: Jan 15 17:32:20 2027 GMT
  host: dhsdigital.eu
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dhsdigital-eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dhsdigital-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: dhsdigital-eu
provider_slug: dhsdigital-eu
slug: dhsdigital-eu-domain-security
source_filename: dhsdigital-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dhsdigital.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 17:32:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: dhsdigital.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dhsdigital-eu/security/dhsdigital-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
