---
api_specs:
- filename: hormonaly-ai-openapi-generated.yml
  format: yaml
  label: hormonaly-ai API
  slug: hormonaly-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hormonaly-ai/openapi/_ae-authored/hormonaly-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hormonaly.ai
  spf: true
hosts:
- cert_expires: Jan 31 20:57:59 2027 GMT
  host: hormonaly.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: hormonaly-ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for hormonaly-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: hormonaly-ai
provider_slug: hormonaly-ai
slug: hormonaly-ai-domain-security
source_filename: hormonaly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hormonaly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 20:57:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hormonaly.ai\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hormonaly-ai/security/hormonaly-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Healthcare
- e-Prescribing
- Medical Education
- Clinical Decision Support
- Longevity Medicine
---
