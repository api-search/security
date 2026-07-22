---
api_specs:
- filename: next-big-idea-club-members-openapi.yml
  format: yaml
  label: Next Big Idea Club Members API
  slug: next-big-idea-club-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/openapi/next-big-idea-club-members-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextbigideaclub.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: nextbigideaclub.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Next Big Idea Club Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Next Big Idea Club, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Next Big Idea Club
provider_slug: next-big-idea-club
slug: next-big-idea-club-domain-security
source_filename: next-big-idea-club-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nextbigideaclub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nextbigideaclub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-big-idea-club/refs/heads/main/security/next-big-idea-club-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Books
- Media
- Subscription
- Nonfiction
- Podcast
- Education
- Membership
---
