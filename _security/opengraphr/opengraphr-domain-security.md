---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: false
  dnssec: false
  domain: opengraphr.com
  spf: false
hosts:
- cert_expires: Sep  4 20:18:08 2026 GMT
  host: opengraphr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opengraphr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenGraphr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenGraphr
provider_slug: opengraphr
slug: opengraphr-domain-security
source_filename: opengraphr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opengraphr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:18:08 2026 GMT\n  hsts: false\ndomains:\n- domain: opengraphr.com\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opengraphr/refs/heads/main/security/opengraphr-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
