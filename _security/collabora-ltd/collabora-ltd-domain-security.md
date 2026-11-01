---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: collabora.com
  spf: true
hosts:
- cert_expires: Dec  9 06:17:54 2026 GMT
  host: www.collabora.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Collabora Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Collabora Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Collabora Ltd.
provider_slug: collabora-ltd
slug: collabora-ltd-domain-security
source_filename: collabora-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.collabora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 06:17:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: collabora.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/collabora-ltd/security/collabora-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- OpenSource
- Consulting
- Software
- Services
---
