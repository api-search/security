---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: screenshotapi.net
  spf: true
hosts:
- cert_expires: Sep 17 10:55:08 2026 GMT
  host: screenshotapi.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Screenshotapi Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScreenshotAPI.net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ScreenshotAPI.net
provider_slug: screenshotapi-net
slug: screenshotapi-net-domain-security
source_filename: screenshotapi-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: screenshotapi.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:55:08 2026 GMT\n  hsts: false\ndomains:\n- domain: screenshotapi.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screenshotapi-net/refs/heads/main/security/screenshotapi-net-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Development
- Public APIs
---
