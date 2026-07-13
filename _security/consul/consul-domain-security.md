---
api_specs:
- filename: consul-http-api.yml
  format: yaml
  label: Consul HTTP API
  slug: http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/openapi/consul-http-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: consul.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hashicorp.com
  spf: true
hosts:
- cert_expires: Sep  3 22:56:23 2026 GMT
  host: www.consul.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 05:45:45 2026 GMT
  host: developer.hashicorp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Consul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HashiCorp Consul, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HashiCorp Consul
provider_slug: consul
slug: consul-domain-security
source_filename: consul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.consul.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 22:56:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.hashicorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:45:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: consul.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hashicorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consul/refs/heads/main/security/consul-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ACL
- Configuration
- Health Checking
- Key/Value Store
- Multi-Datacenter
- Open Source
- Service Discovery
- Service Mesh
---
