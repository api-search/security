---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agingresearch.news
  spf: false
hosts:
- cert_expires: May  6 23:59:59 2027 GMT
  host: agingresearch.news
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agingresearch News Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgingResearch.News, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AgingResearch.News
provider_slug: agingresearch-news
slug: agingresearch-news-domain-security
source_filename: agingresearch-news-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agingresearch.news\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: agingresearch.news\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agingresearch-news/security/agingresearch-news-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Aging
- Longevity
- Artificial Intelligence
- Research
- News
---
