---
api_specs:
- filename: adscrawl-browser-tasks-api-openapi.yml
  format: yaml
  label: AdsCrawl Browser tasks API
  slug: adscrawl-browser-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-browser-tasks-api-openapi.yml
- filename: adscrawl-cloud-browsers-api-openapi.yml
  format: yaml
  label: AdsCrawl Cloud browsers API
  slug: adscrawl-cloud-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-cloud-browsers-api-openapi.yml
- filename: adscrawl-remote-cdp-api-openapi.yml
  format: yaml
  label: AdsCrawl Remote CDP API
  slug: adscrawl-remote-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/openapi/adscrawl-remote-cdp-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adscrawl.net
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.adscrawl.net
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adscrawl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdsCrawl, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AdsCrawl
provider_slug: adscrawl
slug: adscrawl-domain-security
source_filename: adscrawl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adscrawl.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: adscrawl.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adscrawl/refs/heads/main/security/adscrawl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Browser Automation
- WebDataExtraction
- Playwright
- Puppeteer
- Chrome DevTools Protocol
---
