---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: karbach.digital
  spf: true
hosts:
- cert_expires: Jan  6 12:35:10 2027 GMT
  host: karbach.digital
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: karbach-digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for karbach-digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: karbach-digital
provider_slug: karbach-digital
slug: karbach-digital-domain-security
source_filename: karbach-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: karbach.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 12:35:10 2027 GMT\n  hsts: null\ndomains:\n- domain: karbach.digital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/karbach-digital/security/karbach-digital-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
