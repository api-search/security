---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adsuploader.com
  spf: true
hosts:
- cert_expires: Jan 28 02:34:32 2027 GMT
  host: adsuploader.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adsuploader Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ads Uploader, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ads Uploader
provider_slug: adsuploader-com
slug: adsuploader-com-domain-security
source_filename: adsuploader-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adsuploader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 02:34:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adsuploader.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/adsuploader-com/security/adsuploader-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Meta Ads
- Automation
- Bulk Upload
- Creative Testing
- Marketing
---
