---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: discovercloud.com
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.discovercloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Discovercloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DiscoverCloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DiscoverCloud
provider_slug: discovercloud
slug: discovercloud-domain-security
source_filename: discovercloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.discovercloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: discovercloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discovercloud/refs/heads/main/security/discovercloud-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud Services
- Marketplace
- SaaS
- Software Discovery
---
