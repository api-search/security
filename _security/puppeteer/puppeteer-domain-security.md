---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pptr.dev
  spf: true
hosts:
- cert_expires: Sep 15 13:31:21 2026 GMT
  host: pptr.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Puppeteer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Puppeteer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Puppeteer
provider_slug: puppeteer
slug: puppeteer-domain-security
source_filename: puppeteer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pptr.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 13:31:21 2026 GMT\n  hsts: false\ndomains:\n- domain: pptr.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/puppeteer/refs/heads/main/security/puppeteer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Browser Automation
- Headless Browsers
- Scraping
---
