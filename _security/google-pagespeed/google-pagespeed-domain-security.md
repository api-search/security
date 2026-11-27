---
api_specs:
- filename: google-pagespeed-pagespeedapi-api-openapi.yml
  format: yaml
  label: Google PageSpeed Pagespeed Pagespeedapi API
  slug: google-pagespeed-pagespeedapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-pagespeed/openapi/google-pagespeed-pagespeedapi-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: true
  domain: web.dev
  spf: false
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:11:14 2026 GMT
  host: pagespeed.web.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google PageSpeed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google PageSpeed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google PageSpeed
provider_slug: google-pagespeed
slug: google-pagespeed-domain-security
source_filename: google-pagespeed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: pagespeed.web.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:11:14 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: web.dev\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/google-pagespeed/security/google-pagespeed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Core Web Vitals
- Google
- Lighthouse
- Page Speed
- SEO
- Web Performance
---
