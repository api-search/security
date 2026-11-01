---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: is.finance
  spf: false
hosts:
- cert_expires: Dec 30 02:26:58 2026 GMT
  host: is.finance
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Is Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InvestaX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: InvestaX
provider_slug: is-finance
slug: is-finance-domain-security
source_filename: is-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: is.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 02:26:58 2026 GMT\n  hsts: false\ndomains:\n- domain: is.finance\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/is-finance/security/is-finance-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
