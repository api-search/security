---
api_specs:
- filename: openanthropic-com-openapi-generated.yml
  format: yaml
  label: OpenAnthropic API
  slug: openanthropic-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openanthropic-com/openapi/_ae-authored/openanthropic-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Feb  1 15:26:22 2027 GMT
  host: www.anthropic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenAnthropic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAnthropic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenAnthropic
provider_slug: openanthropic-com
slug: openanthropic-com-domain-security
source_filename: openanthropic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 15:26:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anthropic.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/openanthropic-com/security/openanthropic-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- LLM
- Safety
---
