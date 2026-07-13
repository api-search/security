---
api_specs:
- filename: asyncapi.yaml
  format: yaml
  label: Zilla Gateway
  slug: zilla-gateway
  spec_type: AsyncAPI
  url: https://docs.aklivity.io/zilla/latest/concepts/config/
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issue "awstrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aklivity.io
  spf: true
hosts:
- cert_expires: Sep 28 13:36:51 2026 GMT
  host: www.aklivity.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aklivity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aklivity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aklivity
provider_slug: aklivity
slug: aklivity-domain-security
source_filename: aklivity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aklivity.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:36:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aklivity.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aklivity/refs/heads/main/security/aklivity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Gateway
- Apache Kafka
- Event-Driven
- IoT
- Kafka Proxy
- Multi-Protocol
- Real-Time
---
