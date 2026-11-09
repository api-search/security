---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: findmyfarmer.ca
  spf: true
hosts:
- cert_expires: Feb  4 20:46:16 2027 GMT
  host: findmyfarmer.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Findmyfarmer Ca Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for findmyfarmer-ca, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: findmyfarmer-ca
provider_slug: findmyfarmer-ca
slug: findmyfarmer-ca-domain-security
source_filename: findmyfarmer-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findmyfarmer.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 20:46:16 2027 GMT\n  hsts: null\ndomains:\n- domain: findmyfarmer.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/findmyfarmer-ca/security/findmyfarmer-ca-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
