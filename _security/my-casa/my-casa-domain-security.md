---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: my.casa
  spf: true
hosts:
- cert_expires: Dec 12 00:55:20 2026 GMT
  host: my.casa
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: My Casa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Casa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Casa
provider_slug: my-casa
slug: my-casa-domain-security
source_filename: my-casa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: my.casa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 00:55:20 2026 GMT\n  hsts: null\ndomains:\n- domain: my.casa\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/my-casa/security/my-casa-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- SmartHome
- Security
- IoT
- Subscription
---
