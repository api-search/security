---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ailawframework.com
  spf: false
hosts:
- cert_expires: Dec 15 02:10:34 2026 GMT
  host: ailawframework.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ailawframework Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ailawframework-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: ailawframework-com
provider_slug: ailawframework-com
slug: ailawframework-com-domain-security
source_filename: ailawframework-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ailawframework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 02:10:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ailawframework.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ailawframework-com/security/ailawframework-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI policy
- Law firm tools
- Knowledge management
---
