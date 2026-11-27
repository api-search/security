---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freudly.ai
  spf: true
hosts:
- cert_expires: Jan 16 12:47:04 2027 GMT
  host: freudly.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freudly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freudly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freudly
provider_slug: freudly-ai
slug: freudly-ai-domain-security
source_filename: freudly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freudly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 12:47:04 2027 GMT\n  hsts: false\ndomains:\n- domain: freudly.ai\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/freudly-ai/security/freudly-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Psychological Tests
- AI Mental Coach
- Mental Health
- Personality Assessment
- Mood Tracking
- Neurodiversity
- Relationships
---
