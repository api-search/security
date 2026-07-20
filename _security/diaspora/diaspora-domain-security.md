---
api_specs:
- filename: diaspora-api-openapi.yml
  format: yaml
  label: diaspora* API
  slug: diaspora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: diasporafoundation.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: diaspora.social
  spf: true
hosts:
- cert_expires: Sep 15 18:21:43 2026 GMT
  host: diasporafoundation.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 05:26:24 2026 GMT
  host: diaspora.social
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diaspora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diaspora, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Diaspora
provider_slug: diaspora
slug: diaspora-domain-security
source_filename: diaspora-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: diasporafoundation.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:21:43 2026 GMT\n  hsts: false\n- host: diaspora.social\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:26:24 2026 GMT\n  hsts: false\ndomains:\n- domain: diasporafoundation.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: diaspora.social\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/security/diaspora-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Social
- Social Networking
- Decentralized
- Federated
- Open Source
- Privacy
- Fediverse
- Messaging
- OpenID Connect
---
