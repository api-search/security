---
api_specs:
- filename: api.json
  format: json
  label: Ceph RESTful API
  slug: restful-api
  spec_type: OpenAPI
  url: https://{manager_host}:{dashboard_port}/docs/api.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:ceph-infra-admins@redhat.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ceph.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ceph.com
  spf: true
hosts:
- cert_expires: Aug  1 14:48:35 2026 GMT
  host: ceph.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 03:52:16 2026 GMT
  host: docs.ceph.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ceph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ceph, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ceph
provider_slug: ceph
slug: ceph-domain-security
source_filename: ceph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ceph.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 14:48:35 2026 GMT\n  hsts: null\n- host: docs.ceph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:52:16 2026 GMT\n  hsts: false\ndomains:\n- domain: ceph.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:ceph-infra-admins@redhat.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ceph.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceph/refs/heads/main/security/ceph-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Storage
- Distributed Storage
- Object Storage
- Block Storage
- File Storage
- Open Source
- Software-Defined Storage
---
