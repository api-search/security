---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fact-base.com
  spf: false
hosts:
- cert_expires: Sep  1 10:31:15 2026 GMT
  host: fact-base.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fact Base Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fact Base Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fact Base Inc.
provider_slug: fact-base-inc
slug: fact-base-inc-domain-security
source_filename: fact-base-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fact-base.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:31:15 2026 GMT\n  hsts: false\ndomains:\n- domain: fact-base.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fact-base-inc/refs/heads/main/security/fact-base-inc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Manufacturing
- Japan
- Digitization
- Smart Factory
- Manufacturing Technology
- Industry 4.0
---
