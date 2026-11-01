---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: arvancloud.ir
  spf: true
hosts:
- cert_expires: Nov 18 23:15:02 2026 GMT
  host: arvancloud.ir
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arvancloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ArvanCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ArvanCloud
provider_slug: arvancloud
slug: arvancloud-domain-security
source_filename: arvancloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arvancloud.ir\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:15:02 2026 GMT\n  hsts: false\ndomains:\n- domain: arvancloud.ir\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/arvancloud/security/arvancloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- CDN
- Storage
- VideoStreaming
- Security
- Company
---
