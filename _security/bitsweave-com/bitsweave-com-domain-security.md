---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bitsweave.com
  spf: true
hosts:
- cert_expires: Dec 10 17:12:39 2026 GMT
  host: bitsweave.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: bitsweave-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bitsweave-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: bitsweave-com
provider_slug: bitsweave-com
slug: bitsweave-com-domain-security
source_filename: bitsweave-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitsweave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 17:12:39 2026 GMT\n  hsts: null\ndomains:\n- domain: bitsweave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bitsweave-com/security/bitsweave-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
