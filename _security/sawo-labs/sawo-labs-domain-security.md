---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sawolabs.com
  spf: false
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: sawolabs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sawo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAWO Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SAWO Labs
provider_slug: sawo-labs
slug: sawo-labs-domain-security
source_filename: sawo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sawolabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sawolabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sawo-labs/refs/heads/main/security/sawo-labs-domain-security.yml
summary_line: TLSv1.3
tags:
- Authentication And Authorization
- Public APIs
---
