---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: axelrodlabs.com
  spf: true
hosts:
- cert_expires: Dec 17 23:57:21 2026 GMT
  host: axelrodlabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axelrodlabs Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axelrod, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Axelrod
provider_slug: axelrodlabs-com
slug: axelrodlabs-com-domain-security
source_filename: axelrodlabs-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axelrodlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:57:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: axelrodlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/axelrodlabs-com/security/axelrodlabs-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
