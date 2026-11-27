---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ivdframework.dev
  spf: true
hosts:
- cert_expires: Dec 27 04:16:19 2026 GMT
  host: ivdframework.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IVD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IVD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IVD
provider_slug: ivdframework-dev
slug: ivdframework-dev-domain-security
source_filename: ivdframework-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ivdframework.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 04:16:19 2026 GMT\n  hsts: false\ndomains:\n- domain: ivdframework.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ivdframework-dev/security/ivdframework-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- IntentVerification
- Development Tools
- Open Source
- Compliance
---
