---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cohere-technologies.com
  spf: true
hosts:
- cert_expires: Jan 10 05:39:18 2027 GMT
  host: cohere-technologies.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cohere Technologies Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cohere Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cohere Technologies
provider_slug: cohere-technologies-com
slug: cohere-technologies-com-domain-security
source_filename: cohere-technologies-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cohere-technologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 05:39:18 2027 GMT\n  hsts: false\ndomains:\n- domain: cohere-technologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cohere-technologies-com/security/cohere-technologies-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Telecom
- RAN
- 5G
- USM
- Innovation
---
