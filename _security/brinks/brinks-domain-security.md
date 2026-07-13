---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brinks.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brinksinc.com
  spf: true
hosts:
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: us.brinks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: customerportal.brinksinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brinks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brinks, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brinks
provider_slug: brinks
slug: brinks-domain-security
source_filename: brinks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.brinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: false\n- host: customerportal.brinksinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: brinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: brinksinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brinks/refs/heads/main/security/brinks-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cash Management
- Security
- ATM Services
- Financial Services
- Armored Transport
---
