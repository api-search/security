---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: effecthub.net
  spf: true
hosts:
- cert_expires: Jan 12 15:33:55 2027 GMT
  host: effecthub.net
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EffectHub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EffectHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: EffectHub
provider_slug: effecthub-net
slug: effecthub-net-domain-security
source_filename: effecthub-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: effecthub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 15:33:55 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: effecthub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/effecthub-net/security/effecthub-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Catalog
- Tools
- Pricing
- Verification
- Company
---
