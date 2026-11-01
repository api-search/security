---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usetola.com
  spf: true
hosts:
- cert_expires: Jan 11 22:59:23 2027 GMT
  host: usetola.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usetola Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tola, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tola
provider_slug: usetola-com
slug: usetola-com-domain-security
source_filename: usetola-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usetola.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:59:23 2027 GMT\n  hsts: null\ndomains:\n- domain: usetola.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/usetola-com/security/usetola-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
