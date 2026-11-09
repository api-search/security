---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 123rf.com
  spf: true
hosts:
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: www.123rf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 123Rf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 123RF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 123RF
provider_slug: 123rf
slug: 123rf-domain-security
source_filename: 123rf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.123rf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: 123rf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/123rf/security/123rf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Stock Media
- Image
- Vectors
- Video
- Audio
- AI Tools
---
