---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: anglero.com
  spf: true
hosts:
- cert_expires: Dec 18 21:44:50 2026 GMT
  host: anglero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MerkabaPhi AS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MerkabaPhi AS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: MerkabaPhi AS
provider_slug: anglero-com
slug: anglero-com-domain-security
source_filename: anglero-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anglero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 21:44:50 2026 GMT\n  hsts: false\ndomains:\n- domain: anglero.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anglero-com/security/anglero-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Advisory
- Consulting
- Norway
- Leadership
- Company
---
