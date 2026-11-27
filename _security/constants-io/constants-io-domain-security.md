---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: constants.io
  spf: true
hosts:
- cert_expires: Dec 17 03:30:32 2026 GMT
  host: constants.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Constants Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Constants, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Constants
provider_slug: constants-io
slug: constants-io-domain-security
source_filename: constants-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: constants.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 03:30:32 2026 GMT\n  hsts: false\ndomains:\n- domain: constants.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/constants-io/security/constants-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Digital Twin
- Simulation
- Product Analytics
- User Behavior
---
