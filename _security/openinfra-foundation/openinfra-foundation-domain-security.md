---
api_specs:
- filename: openinfra-foundation-openapi.yml
  format: yaml
  label: OpenStack
  slug: openstack
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openinfra-foundation/refs/heads/main/openapi/openinfra-foundation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openinfra.org
  spf: true
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstack.org
  spf: true
hosts:
- cert_expires: Aug 16 22:29:06 2026 GMT
  host: openinfra.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 23:43:47 2026 GMT
  host: www.openstack.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 00:03:57 2026 GMT
  host: katacontainers.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openinfra Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenInfra Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenInfra Foundation
provider_slug: openinfra-foundation
slug: openinfra-foundation-domain-security
source_filename: openinfra-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openinfra.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 22:29:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.openstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: katacontainers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 00:03:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openinfra.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openstack.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openinfra-foundation/refs/heads/main/security/openinfra-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Computing
- Infrastructure
- Linux Foundation
- OpenStack
- Kata Containers
- StarlingX
- Zuul
---
