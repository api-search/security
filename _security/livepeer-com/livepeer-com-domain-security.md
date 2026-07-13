---
api_specs:
- filename: livepeer-studio-openapi.yml
  format: yaml
  label: Livepeer Studio API
  slug: studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-studio-openapi.yml
- filename: livepeer-ai-worker-openapi.yml
  format: yaml
  label: Livepeer AI Network
  slug: ai-network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-ai-worker-openapi.yml
- filename: livepeer-cli-http-openapi.yml
  format: yaml
  label: Livepeer Node CLI HTTP API
  slug: cli-http
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/openapi/livepeer-cli-http-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: livepeer.org
  spf: true
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: livepeer.studio
  spf: true
hosts:
- cert_expires: Sep  9 00:38:56 2026 GMT
  host: livepeer.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 05:48:40 2026 GMT
  host: livepeer.studio
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:16:33 2026 GMT
  host: docs.livepeer.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Livepeer Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Livepeer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Livepeer
provider_slug: livepeer-com
slug: livepeer-com-domain-security
source_filename: livepeer-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: livepeer.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 00:38:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: livepeer.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 05:48:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.livepeer.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:16:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: livepeer.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: livepeer.studio\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc:\
  \ true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/livepeer-com/refs/heads/main/security/livepeer-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Video
- Live Streaming
- Video On Demand
- AI Video
- Decentralized Compute
- GPU Network
- Ethereum
- Arbitrum
- Web3
---
