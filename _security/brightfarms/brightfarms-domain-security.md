---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brightfarms.com
  spf: true
hosts:
- cert_expires: Dec 29 08:48:45 2026 GMT
  host: www.brightfarms.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brightfarms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightFarms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BrightFarms
provider_slug: brightfarms
slug: brightfarms-domain-security
source_filename: brightfarms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightfarms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: brightfarms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightfarms/refs/heads/main/security/brightfarms-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agriculture
- Sustainability
- FreshProduce
- IndoorFarming
---
