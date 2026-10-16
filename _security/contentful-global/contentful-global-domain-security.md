---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: contentful.com
  spf: true
hosts:
- cert_expires: Nov 24 16:06:31 2026 GMT
  host: www.contentful.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contentful Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentful Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Contentful Global
provider_slug: contentful-global
slug: contentful-global-domain-security
source_filename: contentful-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.contentful.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 16:06:31 2026 GMT\n  hsts: null\ndomains:\n- domain: contentful.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentful-global/refs/heads/main/security/contentful-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Content Management
- API
- SaaS
- Cloud
- Salesforce
---
