---
api_specs:
- filename: sociallisteningapi-openapi.yml
  format: yaml
  label: SocialListeningAPI
  slug: sociallisteningapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/openapi/sociallisteningapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sociallisteningapi.com
  spf: false
hosts:
- cert_expires: Nov  2 04:23:39 2026 GMT
  host: sociallisteningapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 06:04:47 2026 GMT
  host: api.sociallisteningapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Sociallisteningapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SocialListeningAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SocialListeningAPI
provider_slug: sociallisteningapi
slug: sociallisteningapi-domain-security
source_filename: sociallisteningapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sociallisteningapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 04:23:39 2026 GMT\n  hsts: false\n- host: api.sociallisteningapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 06:04:47 2026 GMT\n  hsts: false\ndomains:\n- domain: sociallisteningapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sociallisteningapi/refs/heads/main/security/sociallisteningapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Social Listening
- Social Media
- Search
- Brand Monitoring
- Market Research
- MCP
- Reddit
- LinkedIn
---
