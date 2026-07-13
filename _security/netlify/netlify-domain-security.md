---
api_specs:
- filename: netlify-openapi-original.yml
  format: yaml
  label: Netlify API
  slug: netlify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/netlify/refs/heads/main/openapi/netlify-openapi-original.yml
description: ''
domains:
- caa:
  - 128 issue "digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226"
  - 128 issue "amazon.com"
  - 128 iodef "mailto:security@netlify.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netlify.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: app.netlify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: docs.netlify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.netlify.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Netlify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netlify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Netlify
provider_slug: netlify
slug: netlify-domain-security
source_filename: netlify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: app.netlify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.netlify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.netlify.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: netlify.com\n  dnssec: false\n  caa:\n  - 128 issue \"digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226\"\n  - 128 issue \"amazon.com\"\n  - 128 iodef \"mailto:security@netlify.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netlify/refs/heads/main/security/netlify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CDN
- Cloud
- Continuous Deployment
- Edge Computing
- JAMstack
- Serverless
- Serverless Functions
- Static Sites
- Web Hosting
- Websites
---
