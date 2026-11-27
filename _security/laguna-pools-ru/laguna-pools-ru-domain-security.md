---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: laguna-pools.ru
  spf: true
hosts:
- cert_expires: Nov 28 11:43:01 2026 GMT
  host: laguna-pools.ru
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laguna Pools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laguna Pools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Laguna Pools
provider_slug: laguna-pools-ru
slug: laguna-pools-ru-domain-security
source_filename: laguna-pools-ru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laguna-pools.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 11:43:01 2026 GMT\n  hsts: false\ndomains:\n- domain: laguna-pools.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/laguna-pools-ru/security/laguna-pools-ru-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pools
- Manufacturing
- Composite
- Russia
---
