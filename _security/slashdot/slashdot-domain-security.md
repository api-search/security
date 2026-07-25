---
api_specs:
- filename: slashdot-apple-api-openapi.yml
  format: yaml
  label: Slashdot Apple API
  slug: slashdot-apple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-apple-api-openapi.yml
- filename: slashdot-developers-api-openapi.yml
  format: yaml
  label: Slashdot Developers API
  slug: slashdot-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-developers-api-openapi.yml
- filename: slashdot-feeds-api-openapi.yml
  format: yaml
  label: Slashdot Feeds API
  slug: slashdot-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-feeds-api-openapi.yml
- filename: slashdot-games-api-openapi.yml
  format: yaml
  label: Slashdot Games API
  slug: slashdot-games-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-games-api-openapi.yml
- filename: slashdot-linux-api-openapi.yml
  format: yaml
  label: Slashdot Linux API
  slug: slashdot-linux-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-linux-api-openapi.yml
- filename: slashdot-rights-api-openapi.yml
  format: yaml
  label: Slashdot Rights API
  slug: slashdot-rights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-rights-api-openapi.yml
- filename: slashdot-science-api-openapi.yml
  format: yaml
  label: Slashdot Science API
  slug: slashdot-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/openapi/slashdot-science-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:siteops@slashdotmedia.com"
  - 0 issue "sectigo.com"
  - 0 issue "cloudflare.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: slashdot.org
  spf: true
hosts:
- cert_expires: Aug 25 23:54:19 2026 GMT
  host: slashdot.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 23:54:19 2026 GMT
  host: rss.slashdot.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slashdot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slashdot, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Slashdot
provider_slug: slashdot
slug: slashdot-domain-security
source_filename: slashdot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: slashdot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:54:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rss.slashdot.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:54:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: slashdot.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:siteops@slashdotmedia.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slashdot/refs/heads/main/security/slashdot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- Open Source
- Technology News
- RSS
---
