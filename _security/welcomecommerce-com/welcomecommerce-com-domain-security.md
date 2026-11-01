---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: welcomecommerce.com
  spf: true
hosts:
- cert_expires: Jan  5 00:06:50 2027 GMT
  host: welcomecommerce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Welcomecommerce Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Welcome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Welcome
provider_slug: welcomecommerce-com
slug: welcomecommerce-com-domain-security
source_filename: welcomecommerce-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welcomecommerce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 00:06:50 2027 GMT\n  hsts: null\ndomains:\n- domain: welcomecommerce.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/welcomecommerce-com/security/welcomecommerce-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
