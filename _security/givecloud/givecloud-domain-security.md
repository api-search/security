---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: givecloud.com
  spf: true
hosts:
- cert_expires: Dec 11 15:53:35 2026 GMT
  host: givecloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Givecloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Givecloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Givecloud
provider_slug: givecloud
slug: givecloud-domain-security
source_filename: givecloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: givecloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 15:53:35 2026 GMT\n  hsts: false\ndomains:\n- domain: givecloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/givecloud/security/givecloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fundraising
- Nonprofit
- SaaS
- Platform
---
