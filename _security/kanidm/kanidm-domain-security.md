---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kanidm.com
  spf: false
hosts:
- cert_expires: Nov 26 20:18:21 2026 GMT
  host: kanidm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kanidm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kanidm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kanidm
provider_slug: kanidm
slug: kanidm-domain-security
source_filename: kanidm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kanidm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 20:18:21 2026 GMT\n  hsts: false\ndomains:\n- domain: kanidm.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kanidm/security/kanidm-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Identity
- Authentication
- OpenSource
- Rust
---
