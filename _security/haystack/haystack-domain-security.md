---
description: ''
domains:
- caa:
  - 0 iodef "mailto:domains@deepset.ai"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deepset.ai
  spf: true
hosts:
- cert_expires: Sep 18 07:13:51 2026 GMT
  host: haystack.deepset.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Haystack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Haystack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Haystack
provider_slug: haystack
slug: haystack-domain-security
source_filename: haystack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: haystack.deepset.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:13:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: deepset.ai\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domains@deepset.ai\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/haystack/refs/heads/main/security/haystack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Automation
- LLM Framework
---
