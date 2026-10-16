---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boltfoundry.com
  spf: true
hosts:
- cert_expires: Dec  9 21:18:49 2026 GMT
  host: boltfoundry.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boltfoundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt Foundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bolt Foundry
provider_slug: boltfoundry
slug: boltfoundry-domain-security
source_filename: boltfoundry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boltfoundry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 21:18:49 2026 GMT\n  hsts: null\ndomains:\n- domain: boltfoundry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltfoundry/refs/heads/main/security/boltfoundry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
