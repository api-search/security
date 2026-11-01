---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spicecsm.com
  spf: true
hosts:
- cert_expires: Mar 27 23:59:59 2027 GMT
  host: spicecsm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Spicecsm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpiceCSM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SpiceCSM
provider_slug: spicecsm
slug: spicecsm-domain-security
source_filename: spicecsm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spicecsm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: spicecsm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/spicecsm/security/spicecsm-domain-security.yml
summary_line: TLSv1.3
tags:
- Customer Success
- Software-as-a-Service
- Platform
- Automation
- Analytics
---
