---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: likebucket.com
  spf: true
hosts:
- cert_expires: Feb 23 15:32:47 2027 GMT
  host: likebucket.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Likebucket Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bucket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bucket
provider_slug: likebucket-com
slug: likebucket-com-domain-security
source_filename: likebucket-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: likebucket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 15:32:47 2027 GMT\n  hsts: null\ndomains:\n- domain: likebucket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/likebucket-com/security/likebucket-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Cloud
- Storage
- FileSharing
- API
- DeveloperTools
---
