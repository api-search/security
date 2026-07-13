---
api_specs:
- filename: haproxy_spec.yaml
  format: yaml
  label: HAProxy Data Plane API
  slug: haproxy
  spec_type: OpenAPI
  url: https://github.com/haproxytech/dataplaneapi/blob/master/specification/build/haproxy_spec.yaml
- filename: management-api.json
  format: json
  label: RabbitMQ Management API
  slug: rabbitmq
  spec_type: OpenAPI
  url: https://www.rabbitmq.com/resources/specs/management-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: haproxy.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: docs.aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.haproxy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 18:18:03 2026 GMT
  host: upstash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalable Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalable Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scalable Systems
provider_slug: scalable-systems
slug: scalable-systems-domain-security
source_filename: scalable-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: www.haproxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\n- host: upstash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:18:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: haproxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-systems/refs/heads/main/security/scalable-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Scaling
- Caching
- Cloud Infrastructure
- Distributed Systems
- High Availability
- Infrastructure
- Load Balancing
- Message Queues
- Platform Engineering
- Scalable Architecture
- Service Discovery
---
