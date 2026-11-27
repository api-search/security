---
api_specs:
- filename: wavegrain-com-openapi-generated.yml
  format: yaml
  label: Wavegrain API
  slug: wavegrain-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wavegrain-com/openapi/_ae-authored/wavegrain-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wavegrain.com
  spf: true
hosts:
- cert_expires: Feb  2 18:38:02 2027 GMT
  host: wavegrain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wavegrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wavegrain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Wavegrain
provider_slug: wavegrain-com
slug: wavegrain-com-domain-security
source_filename: wavegrain-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wavegrain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 18:38:02 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wavegrain.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/wavegrain-com/security/wavegrain-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Automation
- Social Media
- TikTok
- Instagram
---
