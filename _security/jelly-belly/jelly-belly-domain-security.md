---
api_specs:
- filename: jelly-belly-openapi.yml
  format: yaml
  label: Jelly Belly Wiki API
  slug: jelly-belly-wiki-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jelly-belly/refs/heads/main/openapi/jelly-belly-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jellybelly.com
  spf: true
- caa:
  - 128 iodef "mailto:security@netlify.com"
  - 128 issue "digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: netlify.app
  spf: true
hosts:
- cert_expires: Aug 30 14:32:03 2026 GMT
  host: www.jellybelly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: jelly-belly-wiki.netlify.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 22:01:50 2026 GMT
  host: jellybellywikiapi.onrender.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jelly Belly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jelly Belly, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jelly Belly
provider_slug: jelly-belly
slug: jelly-belly-domain-security
source_filename: jelly-belly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jellybelly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:32:03 2026 GMT\n  hsts: false\n- host: jelly-belly-wiki.netlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: jellybellywikiapi.onrender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 22:01:50 2026 GMT\n  hsts: null\ndomains:\n- domain: jellybelly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: netlify.app\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:security@netlify.com\"\n  - 128 issue \"digicert.com;account=2d83e9ac9b6776c3f215150f6ebceea8cefe3bc2e1fb5efffb1d71e200575226\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jelly-belly/refs/heads/main/security/jelly-belly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beans
- Candy
- Confectionery
- Food
- Jelly Beans
- Recipes
---
