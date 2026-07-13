---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Lemmy REST API
  slug: api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: join-lemmy.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lemmy.world
  spf: true
hosts:
- cert_expires: Oct  4 13:59:52 2026 GMT
  host: join-lemmy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 02:33:53 2026 GMT
  host: lemmy.world
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lemmy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lemmy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lemmy
provider_slug: lemmy
slug: lemmy-domain-security
source_filename: lemmy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: join-lemmy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 13:59:52 2026 GMT\n  hsts: false\n- host: lemmy.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 02:33:53 2026 GMT\n  hsts: false\ndomains:\n- domain: join-lemmy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: lemmy.world\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemmy/refs/heads/main/security/lemmy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Communities
- Federated
- Fediverse
- Link Aggregator
- Open-Source
- Social Networks
---
