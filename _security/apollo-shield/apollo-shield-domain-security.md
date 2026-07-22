---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apolloshield.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.apolloshield.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apollo Shield Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apollo Shield, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Apollo Shield
provider_slug: apollo-shield
slug: apollo-shield-domain-security
source_filename: apollo-shield-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apolloshield.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: apolloshield.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-shield/refs/heads/main/security/apollo-shield-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Counter-Drone
- Counter-UAS
- Drone Detection
- Airspace Security
- Physical Security
- Defense Technology
- RF Sensors
---
