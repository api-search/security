---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fetchfox.net
  spf: true
hosts:
- cert_expires: Jan  8 07:35:50 2027 GMT
  host: fetchfox.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fetchfox Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fetchfox-net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fetchfox-net
provider_slug: fetchfox-net
slug: fetchfox-net-domain-security
source_filename: fetchfox-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fetchfox.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 07:35:50 2027 GMT\n  hsts: false\ndomains:\n- domain: fetchfox.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/fetchfox-net/security/fetchfox-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social Data
- API
- Media
- YouTube
- Instagram
- TikTok
---
