---
api_specs:
- filename: pagespeed-insights-openapi.yml
  format: yaml
  label: PageSpeed Insights API
  slug: pagespeed-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/openapi/pagespeed-insights-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: true
  domain: web.dev
  spf: false
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Sep 14 08:40:21 2026 GMT
  host: pagespeed.web.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Pagespeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google PageSpeed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Google PageSpeed
provider_slug: google-pagespeed
slug: google-pagespeed-domain-security
source_filename: google-pagespeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagespeed.web.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:40:21 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: web.dev\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-pagespeed/refs/heads/main/security/google-pagespeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
---
