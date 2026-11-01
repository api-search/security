---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: phantomjscloud.com
  spf: true
hosts:
- cert_expires: Jan 12 21:49:52 2027 GMT
  host: phantomjscloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Phantomjscloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PhantomJS Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PhantomJS Cloud
provider_slug: phantomjscloud
slug: phantomjscloud-domain-security
source_filename: phantomjscloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phantomjscloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 21:49:52 2027 GMT\n  hsts: false\ndomains:\n- domain: phantomjscloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/phantomjscloud/security/phantomjscloud-domain-security.yml
summary_line: TLSv1.3
tags:
- Browser API
- Web Scraping
- Rendering
- Automation
- Cloud Service
---
