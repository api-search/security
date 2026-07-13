---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: localclarity.com
  spf: true
hosts:
- cert_expires: Sep 15 00:13:35 2026 GMT
  host: www.localclarity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 05:00:48 2026 GMT
  host: dev.localclarity.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Localclarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LocalClarity, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LocalClarity
provider_slug: localclarity
slug: localclarity-domain-security
source_filename: localclarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.localclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:13:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: dev.localclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 05:00:48 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: localclarity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/localclarity/refs/heads/main/security/localclarity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Local SEO
- Google Business Profile
- Review Management
- Local Search
- Listings Management
- Reputation Management
---
