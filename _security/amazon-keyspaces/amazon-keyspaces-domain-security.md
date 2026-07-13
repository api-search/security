---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amazon Keyspaces API
  slug: amazon-keyspaces-api
  spec_type: OpenAPI
  url: https://api.apis.guru/v2/specs/amazonaws.com/keyspaces/2022-02-10/openapi.yaml
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
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: cassandra.amazonaws.com
  https: false
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: cassandra.us-east-1.amazonaws.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amazon Keyspaces Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon Keyspaces, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon Keyspaces
provider_slug: amazon-keyspaces
slug: amazon-keyspaces-domain-security
source_filename: amazon-keyspaces-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: cassandra.amazonaws.com\n  https: false\n- host: cassandra.us-east-1.amazonaws.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-keyspaces/refs/heads/main/security/amazon-keyspaces-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cassandra
- Database
- Managed Database
- NoSQL
- Wide Column
---
