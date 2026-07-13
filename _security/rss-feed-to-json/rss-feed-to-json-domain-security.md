---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vercel.app
  spf: true
hosts:
- cert_expires: Sep 26 13:27:56 2026 GMT
  host: rss-to-json-serverless-api.vercel.app
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rss Feed To Json Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RSS feed to JSON, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RSS feed to JSON
provider_slug: rss-feed-to-json
slug: rss-feed-to-json-domain-security
source_filename: rss-feed-to-json-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rss-to-json-serverless-api.vercel.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 13:27:56 2026 GMT\n  hsts: null\ndomains:\n- domain: vercel.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rss-feed-to-json/refs/heads/main/security/rss-feed-to-json-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- Public APIs
---
