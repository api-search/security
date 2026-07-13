---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nachonacho.com
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.nachonacho.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nachonacho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NachoNacho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NachoNacho
provider_slug: nachonacho
slug: nachonacho-domain-security
source_filename: nachonacho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nachonacho.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nachonacho.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nachonacho/refs/heads/main/security/nachonacho-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- SaaS Procurement
- Subscription Management
---
