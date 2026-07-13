---
api_specs:
- filename: openstack-keystone-openapi.yml
  format: yaml
  label: OpenStack Identity (Keystone) API
  slug: keystone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-keystone-openapi.yml
- filename: openstack-nova-openapi.yml
  format: yaml
  label: OpenStack Compute (Nova) API
  slug: nova
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-nova-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openstack.org
  spf: true
hosts:
- cert_expires: Sep 17 23:43:47 2026 GMT
  host: www.openstack.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:11:11 2026 GMT
  host: docs.openstack.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenStack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenStack
provider_slug: openstack
slug: openstack-domain-security
source_filename: openstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:43:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openstack.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:11:11 2026 GMT\n  hsts: false\ndomains:\n- domain: openstack.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/security/openstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Platform
- Infrastructure as a Service
- Open Source
- Virtualization
- Linux Foundation
---
