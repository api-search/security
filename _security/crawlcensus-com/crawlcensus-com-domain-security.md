---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crawlcensus.com
  spf: true
hosts:
- cert_expires: Jan 18 02:58:17 2027 GMT
  host: crawlcensus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crawl Census Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crawl Census, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crawl Census
provider_slug: crawlcensus-com
slug: crawlcensus-com-domain-security
source_filename: crawlcensus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crawlcensus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 02:58:17 2027 GMT\n  hsts: false\ndomains:\n- domain: crawlcensus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/crawlcensus-com/security/crawlcensus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Crawlers
- Robots.txt
- SEO
- Web Measurement
- Open Data
- Llms.txt
- MCP
---
