---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chibitek.com
  spf: true
hosts:
- cert_expires: Dec 17 22:35:26 2026 GMT
  host: chibitek.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chibitek Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for chibitek-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: chibitek-com
provider_slug: chibitek-com
slug: chibitek-com-domain-security
source_filename: chibitek-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chibitek.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 22:35:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: chibitek.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/chibitek-com/security/chibitek-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Managed Services
- IT Support
- Cloud
---
