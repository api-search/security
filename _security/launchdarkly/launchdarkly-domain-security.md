---
api_specs:
- filename: launchdarkly-rest-api-openapi.yml
  format: yaml
  label: LaunchDarkly REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/openapi/launchdarkly-rest-api-openapi.yml
- filename: launchdarkly-webhooks-asyncapi.yml
  format: yaml
  label: LaunchDarkly Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/asyncapi/launchdarkly-webhooks-asyncapi.yml
- filename: launchdarkly-relay-proxy-openapi.yml
  format: yaml
  label: LaunchDarkly Relay Proxy
  slug: relay-proxy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/openapi/launchdarkly-relay-proxy-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: launchdarkly.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: apidocs.launchdarkly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 10 01:05:15 2027 GMT
  host: app.launchdarkly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 18:38:05 2026 GMT
  host: launchdarkly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Launchdarkly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for launchdarkly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: launchdarkly
provider_slug: launchdarkly
slug: launchdarkly-domain-security
source_filename: launchdarkly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apidocs.launchdarkly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.launchdarkly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 01:05:15 2027 GMT\n  hsts: null\n- host: launchdarkly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:38:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: launchdarkly.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchdarkly/refs/heads/main/security/launchdarkly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
