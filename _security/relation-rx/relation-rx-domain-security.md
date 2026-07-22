---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: relationrx.com
  spf: true
hosts:
- cert_expires: Aug 31 19:37:23 2026 GMT
  host: www.relationrx.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relation Rx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relation Rx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Relation Rx
provider_slug: relation-rx
slug: relation-rx-domain-security
source_filename: relation-rx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.relationrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:37:23 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: relationrx.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relation-rx/refs/heads/main/security/relation-rx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Drug Discovery
- Machine Learning
- Genomics
- Multi-omics
- Therapeutics
- Life Sciences
---
