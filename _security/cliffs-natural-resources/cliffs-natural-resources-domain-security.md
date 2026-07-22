---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: clevelandcliffs.com
  spf: true
hosts:
- cert_expires: Sep 20 19:04:39 2026 GMT
  host: www.clevelandcliffs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cliffs Natural Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cliffs Natural Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cliffs Natural Resources
provider_slug: cliffs-natural-resources
slug: cliffs-natural-resources-domain-security
source_filename: cliffs-natural-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clevelandcliffs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:04:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clevelandcliffs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cliffs-natural-resources/refs/heads/main/security/cliffs-natural-resources-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Iron Ore
- Manufacturing
- Mining
- Steel
- Steelmaking
---
