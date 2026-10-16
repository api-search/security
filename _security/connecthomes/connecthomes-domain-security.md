---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: connecthomes.io
  spf: false
hosts:
- cert_expires: Apr  7 23:59:59 2027 GMT
  host: www.connecthomes.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connecthomes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connecthomes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Connecthomes
provider_slug: connecthomes
slug: connecthomes-domain-security
source_filename: connecthomes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connecthomes.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: connecthomes.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connecthomes/refs/heads/main/security/connecthomes-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real Estate
- Prefab Housing
- Sustainable
- Modular Homes
- API Platform
---
