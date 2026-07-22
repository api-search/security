---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sheswell.co
  spf: false
hosts:
- cert_expires: Sep 10 05:46:44 2026 GMT
  host: sheswell.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 28 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 28 labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 28 labs
provider_slug: 28-labs
slug: 28-labs-domain-security
source_filename: 28-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sheswell.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 05:46:44 2026 GMT\n  hsts: false\ndomains:\n- domain: sheswell.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/28-labs/refs/heads/main/security/28-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fertility
- Healthcare
- Digital Health
- Femtech
- Subscription
- Consumer
---
