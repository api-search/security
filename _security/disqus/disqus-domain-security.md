---
api_specs:
- filename: disqus-openapi.yml
  format: yaml
  label: Disqus Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/openapi/disqus-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: disqus.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: disqus.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disqus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Disqus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Disqus
provider_slug: disqus
slug: disqus-domain-security
source_filename: disqus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: disqus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: disqus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disqus/refs/heads/main/security/disqus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Comments
- Community
- Discussions
- Publishing
- Audience Engagement
- Social
---
