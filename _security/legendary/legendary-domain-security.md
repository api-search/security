---
api_specs:
- filename: legendary-wp-rest-openapi.yml
  format: yaml
  label: Legendary Entertainment WordPress REST API
  slug: legendary-wp-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legendary/refs/heads/main/openapi/legendary-wp-rest-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: legendary.com
  spf: true
hosts:
- cert_expires: Sep 29 09:15:23 2026 GMT
  host: www.legendary.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Legendary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Legendary Entertainment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Legendary Entertainment
provider_slug: legendary
slug: legendary-domain-security
source_filename: legendary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.legendary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:15:23 2026 GMT\n  hsts: false\ndomains:\n- domain: legendary.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legendary/refs/heads/main/security/legendary-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Media
- Entertainment
- Film
- Television
- Comics
- Content
- Publishing
- WordPress
---
