---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ombo.cl
  spf: true
hosts:
- cert_expires: Feb 12 20:28:28 2027 GMT
  host: ombo.cl
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ombo-cl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ombo-cl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ombo-cl
provider_slug: ombo-cl
slug: ombo-cl-domain-security
source_filename: ombo-cl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ombo.cl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 20:28:28 2027 GMT\n  hsts: null\ndomains:\n- domain: ombo.cl\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ombo-cl/security/ombo-cl-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
