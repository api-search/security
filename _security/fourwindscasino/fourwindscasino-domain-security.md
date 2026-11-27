---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fourwindscasino.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.fourwindscasino.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Four Winds Casinos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Four Winds Casinos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Four Winds Casinos
provider_slug: fourwindscasino
slug: fourwindscasino-domain-security
source_filename: fourwindscasino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fourwindscasino.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: fourwindscasino.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fourwindscasino/security/fourwindscasino-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Casinos
- Hotels
- Gaming
- Sportsbook
- Dining
- Entertainment
- Players Club
---
