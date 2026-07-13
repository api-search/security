---
api_specs:
- filename: v2-public.yaml
  format: yaml
  label: Wappalyzer Lookup API
  slug: wappalyzer-lookup-api
  spec_type: OpenAPI
  url: https://www.wappalyzer.com/openapi/v2-public.yaml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wappalyzer.com
  spf: true
hosts:
- cert_expires: Sep 11 05:52:04 2026 GMT
  host: www.wappalyzer.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 05:52:04 2026 GMT
  host: api.wappalyzer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wappalyzer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wappalyzer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wappalyzer
provider_slug: wappalyzer
slug: wappalyzer-domain-security
source_filename: wappalyzer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wappalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:52:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wappalyzer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:52:04 2026 GMT\n  hsts: false\ndomains:\n- domain: wappalyzer.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/security/wappalyzer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Technology Detection
- Technographics
- Website Analysis
- CMS Detection
- Framework Detection
- Lead Enrichment
- Sales Intelligence
---
