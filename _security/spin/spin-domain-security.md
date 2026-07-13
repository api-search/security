---
description: ''
domains:
- caa:
  - cloud-loadbalancer.fermyon.com.
  - tf-lb-20230512100548813600000002-56f33b69e309d1c9.elb.us-east-1.amazonaws.com.
  dmarc: false
  dnssec: true
  domain: spinframework.dev
  spf: false
hosts:
- cert_expires: Sep 19 04:44:42 2026 GMT
  host: spinframework.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Spin
provider_slug: spin
slug: spin-domain-security
source_filename: spin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spinframework.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 04:44:42 2026 GMT\n  hsts: false\ndomains:\n- domain: spinframework.dev\n  dnssec: true\n  caa:\n  - cloud-loadbalancer.fermyon.com.\n  - tf-lb-20230512100548813600000002-56f33b69e309d1c9.elb.us-east-1.amazonaws.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spin/refs/heads/main/security/spin-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Cloud Native
- Microservices
- Serverless
- WebAssembly
---
