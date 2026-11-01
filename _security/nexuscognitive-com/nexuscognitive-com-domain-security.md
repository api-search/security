---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nexuscognitive.com
  spf: true
hosts:
- cert_expires: Dec  7 20:54:01 2026 GMT
  host: www.nexuscognitive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nexuscognitive Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexus One, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nexus One
provider_slug: nexuscognitive-com
slug: nexuscognitive-com-domain-security
source_filename: nexuscognitive-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nexuscognitive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 20:54:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nexuscognitive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nexuscognitive-com/security/nexuscognitive-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- AI
- Platform
- Integration
---
